<template>
  <div class="text-8xl emoji-of-the-day">{{ randomEmoji }}</div>
</template>

<script>
export default {
  data() {
    const possibleEmojis = [
      "🚀",
      "👨‍💻",
      "🎉",
      "🌱",
      "🌿",
      "🌳",
      "🌴",
      "🌵",
      "🌾",
      "🌿",
      "🍀",
      "🍁",
      "🍂",
      "🍃",
      "🍄",
      "🌰",
      "🌱",
      "🌲",
      "🌳",
      "🌴",
      "🌵",
      "🌾",
      "🌿",
      "🍀",
      "🍁",
      "🍂",
      "🍃",
      "🍄",
      "🌰",
      "🌱",
      "🌲",
      "🌳",
      "🌴",
      "🌵",
      "🌾",
      "🌿",
      "🍀",
      "🍁",
      "🍂",
      "🍃",
      "🍄",
      "🌰",
      "🌱",
      "🌲",
      "🌳",
      "🌴",
      "🌵",
      "🌾",
      "🌿",
      "🍀",
      "🍁",
      "🍂",
      "🍃",
      "🍄",
      "🌰",
      "🌱",
      "🌲",
      "🌳",
      "🌴",
      "🌵",
      "🌾",
      "🌿",
      "🍀",
      "🍁",
      "🍂",
      "🍃",
      "🍄",
      "🌰",
      "🌱",
      "🌲",
      "🌳",
      "🌴",
      "🌵",
      "🌾",
      "🌿",
      "🍀",
      "🍁",
      "🍂",
      "🍃",
      "🍄",
      "🌰",
      "🌱",
      "🌲",
      "🌳",
      "🌴",
    ];

    const isServer = typeof window === "undefined";
    let randomEmoji = "";
    if (isServer) {
      randomEmoji =
        possibleEmojis[Math.floor(Math.random() * possibleEmojis.length)];
    }
    return { randomEmoji };
  },
};
</script>

<style lang="scss" scoped></style>
