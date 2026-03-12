---
name: multi-platform-distributor
description: Format and optimize content for different platforms
---

# Multi-Platform Distributor

**Purpose**: Format and optimize content for different platforms
**Platforms**: Twitter, Instagram, TikTok, YouTube, Facebook, LinkedIn
**Version**: 1.0.0

## Core Capabilities

- Platform-specific formatting
- Metadata optimization
- Hashtag and keyword strategy
- Cross-platform publishing
- Engagement tracking
- A/B testing support

## Platform Specifications

**Twitter/X**:
- Text: 280 characters
- Media: Images 16:9 or square, video 2:20 max
- Best practices: Thread format for longer stories, hashtags (2-3 max)

**Instagram**:
- Feed: Square or 4:5 vertical
- Stories: 9:16 vertical, 15s clips
- Reels: 9:16 vertical, 90s max
- Captions: First 125 chars critical

**TikTok**:
- Format: 9:16 vertical
- Length: 60s optimal (up to 10 min)
- Captions: Always include
- Sound: Trending audio boost discovery

**YouTube**:
- Format: 16:9 horizontal
- Length: Any (8-12 min optimal for monetization)
- Thumbnails: 1280x720, high contrast
- Chapters: Add for long videos

**Facebook**:
- Video: Square or vertical (mobile)
- Text: Shorter performs better
- Captions: Essential (85% watch without sound)


## Automation Workflow

```python
def distribute_story_multiplatform(story_content, media_files):
    """
    Automated multi-platform distribution
    """
    distribution_plan = {}

    # Twitter thread
    distribution_plan['twitter'] = {
        'format': 'thread',
        'content': create_twitter_thread(story_content),
        'media': optimize_for_twitter(media_files)
    }

    # Instagram carousel
    distribution_plan['instagram'] = {
        'format': 'carousel',
        'images': create_instagram_carousel(story_content),
        'caption': create_instagram_caption(story_content)
    }

    # TikTok video
    if has_video_content(media_files):
        distribution_plan['tiktok'] = {
            'format': 'video',
            'video': format_for_tiktok(media_files['video']),
            'caption': create_tiktok_caption(story_content)
        }

    # YouTube video
    distribution_plan['youtube'] = {
        'format': 'video',
        'video': format_for_youtube(media_files['video']),
        'title': create_youtube_title(story_content),
        'description': create_youtube_description(story_content),
        'thumbnail': generate_thumbnail(story_content)
    }

    # Execute distribution
    for platform, content in distribution_plan.items():
        publish_to_platform(platform, content)

    return distribution_plan
```


## Integration

- Works with **story-editor** for final content
- Coordinates with **video-journalist** for video formatting
- Partners with **seo-optimization-specialist** for discoverability
