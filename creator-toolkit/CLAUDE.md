# Creator Toolkit

AI-powered content creation assistant for Chinese content creators. Two invocable skills for topic discovery and multi-platform content adaptation.

## Skills

- `/topic-finder` — Discover trending topics from Douyin, Xiaohongshu, Weibo, and web searches. Outputs 3-5 topic suggestions with heat scores and angles.
- `/content-adapter` — Adapt a selected topic into platform-optimized copy for Douyin, Xiaohongshu, and Bilibili simultaneously.

## Configuration

Edit `config/source-config.md` to set your niche, preferred platforms, and style preferences. No coding required.

## Usage

1. Clone or copy this folder into your project
2. Edit `config/source-config.md` with your niche and preferences
3. In Claude Code, type `/topic-finder <your niche> 找3个选题`
4. Pick a topic, then type `/content-adapter <selected topic>`
5. Copy the generated copy to your platform

## Requirements

- Claude Code with WebSearch and Skill tools enabled
- No API keys, no database, no install
