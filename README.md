# AI Dodge

A browser-based dodge game built with **Phaser.js 3.60** and **DeepSeek V4 Flash**.

**Play it now:** https://aigamingdev.com/games/ai-dodge/

## How to Play

- Move: **WASD** or arrow keys
- Dodge the red AI hunters
- Survive as long as possible
- Press **R** to restart after game over

## How It Was Built

See the full blog post: https://aigamingdev.com/blog/ai-dodge-tutorial/

The game was built iteratively with AI assistance:
- **Engine:** Phaser.js 3.60 with Arcade Physics
- **AI Model:** DeepSeek V4 Flash
- **Total cost:** ~$0.02 in API usage
- **Total iterations:** 5 prompt-response cycles

## Local Development

```bash
# Serve locally
python3 -m http.server 8000
# Open http://localhost:8000/games/ai-dodge/
```

## License

MIT
