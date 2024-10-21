<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/deed.en"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This sound library is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/deed.en">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

**This repository is the official GitHub repository of the Lingyuosa Creation Group's official account for its Diffsinger sound library's formal repo**

See the [Changelog](https://github.com/yousa-ling-official-production/yousa-ling-diffsinger-v1/blob/main/CHANGELOG.md) for changes.

# yousa-ling-diffsinger-v1
Lingyuosa's Diffsinger model version 1

Based on the [Diffsinger Project](https://github.com/openvpi/DiffSinger)

Check out our [demo and distribution video](https://www.bilibili.com/video/BV1cC4y1o7wE) on BiliBili!

Voice source & chorus demo with the AI [【泠鸢&AI】与自己的ai音源合唱，你能分辨嘛？《时光洪流》【原唱：程响】](https://www.bilibili.com/video/BV1oE421N7eM/)

Japanese demo [中秋泠鸢自愿加班的唱了《乐意效劳》（能听出来嘛~）](https://www.bilibili.com/video/BV1jUt4eAEwj/)

**Model files can be downloaded in the Release section on the right**

## Terms of Use
The following refers to the Diffsinger Lingyuosa AI Sound Library V1.0

1. Works synthesized using this sound library must comply with laws and regulations (cannot be used to generate content that harms the reputation of any person or organization, or to generate illegal audio, etc.).

2. Non-commercial use (not for profit and not charging any fees to third parties) is free of charge.

3. If an individual user generates a work using this sound library to win a prize in a competition or publishes a work on a public platform for free and receives platform incentive earnings without marketing content, it is considered non-commercial use.

## Related Documentation

Usage tutorials: https://diffsinger.com/

OpenUtau: https://github.com/stakira/OpenUtau

Tone division based on: https://github.com/KakaruHayate/ColorSplitter

Dictionary scheme refers to the "Multilingual Usage Instructions.pdf" in the sound library folder

## Additional Notes

Based on the data, some special annotations have been made, which can be used as appropriate

Excessively short `b, p, d, t, g, k` are annotated as `.b, .p, .d, .t, .g, .k`

Extra annotations for Chinese "yár" (~iar) and "wánr" (~uar/uanr) sounds, you can use them with `iar`, `uanr`

End breaths are annotated, you can use `EP` at the end of sentences

Initial `m`, `n` in sentences are annotated, you can use `_m`, `_n` to apply them

You can modify the `character.yaml` and `character.txt` to change the character images and avatars. The `image` folder contains a set of replacement images for character illustrations and avatars
