# seeddanceai

SeedDance ([seeddance.ai](https://seeddance.ai)) is an AI video and image studio. Create clips from text, images, reference video, or audio, then edit, extend, or upscale them, or reverse a result back into a prompt. Credits, task history, and the workspace are shared across models.

Website: [https://seeddance.ai](https://seeddance.ai)

## What you can do

| Tool | Link | Use |
| --- | --- | --- |
| AI Video Generator | [/ai-video-generator](https://seeddance.ai/ai-video-generator) | Text-to-video, image-to-video, reference-to-video |
| AI Image Generator | [/ai-image-generator](https://seeddance.ai/ai-image-generator) | Text-to-image and reference-image edits |
| AI Audio / Music | [/ai-audio-generator](https://seeddance.ai/ai-audio-generator), [/ai-music-generator](https://seeddance.ai/ai-music-generator) | Scene audio and songs |
| AI Video Editor | [/ai-video-editor](https://seeddance.ai/ai-video-editor) | Change a clip from a prompt and keep the rest |
| AI Video Extender | [/ai-video-extender](https://seeddance.ai/ai-video-extender) | Continue a shot forward or backward |
| Video Upscaler | [/video-upscaler](https://seeddance.ai/video-upscaler) | Raise resolution, up to 4K |
| Video to Prompt / Image to Prompt | [/video-to-prompt](https://seeddance.ai/video-to-prompt), [/image-to-prompt](https://seeddance.ai/image-to-prompt) | Extract a reusable prompt from a clip or image |

Models include Seedance 2.5 / 2.5 Flash, Seedance 2.0, Kling, Veo, Gemini, GPT Image, Grok Imagine, and Seedream. After you sign in, switch models and settings in [Studio](https://seeddance.ai/app).

## Examples

**Ad drafts.** Write one product line, render several 5–8 second 720p takes with Seedance 2.5 Flash, then finish the chosen shot in Seedance 2.5 at a higher resolution.

**Image to video.** Upload a product or character still and describe the camera move, for example “the camera slowly pushes in as the person turns toward the lens.” One image is the first frame; two images are the first and last frames.

**Reference to video.** Upload a character image, a motion clip, and background music. In the prompt, point at each file with `@image1`, `@video1`, and `@audio1` so the new shot keeps the same subject and rhythm.

**Edit an existing clip.** In the video editor, upload the source and write “replace the product in @video1 with @image1 and leave everything else unchanged.” Duration and aspect ratio follow the source.

**Vertical social clips.** Generate a 9:16 clip with synced audio, keep it under 15 seconds, then use the video extender when you need a second half.

**Reverse a reference.** Drop a clip or poster into Video to Prompt or Image to Prompt, then take the description back to the generator and swap in your own subject and brand.

## Local development

```bash
pnpm install
pnpm dev
```

The dev server runs at [http://localhost:3000](http://localhost:3000). Generate and apply database migrations with `pnpm db:generate` and `pnpm db:migrate`.
