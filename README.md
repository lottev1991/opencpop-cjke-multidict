<p align="center">
    <img src="images/icon.svg" width="150" height="auto" alt="Model icon">
</p>

<h1 align="center">Opencpop -CJKE Multidict-</h1>
**Opencpop -CJKE Multidict-** is a quadrilingual, multi-dictionary [Diffsinger](https://github.com/openvpi/diffsinger) model trained on the Opencpop dataset (as well as several others used for parallel training; see below).
"CJKE" stands for "Chinese, Japanese, Korean, English". I use the pronunciation "cake" (using the second letter "A" in the word "Japanese" rather than the first letter "J").

Please refer to the [Terms of Use](ToU_EN.md) documents included with this release. The Terms of Use are multilingual, making use of machine translation for non-English languages. Apologies for any translation errors.

**IMPORTANT NOTICE:** This model is ***STRICTLY FOR NON-COMMERCIAL USE ONLY***. If you still wish to use this model for commercial projects, you'll need to contact the Opencpop Team for permission; note that fees may apply.

## Model information
### Supported embeds
- Duration;
- Pitch;
- Random pitch shifting (gender);
- Velocity;
- Multi-dictionary;
### Supported languages
- Mandarin Chinese (primary);
- English;
- Japanese;
- Korean;
### Phonetic systems used:
- Chinese: opencpop-extended;
- English: ARPABET (basic phonemes only);
- Japanese: NNSVS-style;
- Korean: NNSVS-style;
### Additional phonemes
 - `EXH` (exhale sound);
- `cl` (various uses, such as glottal stop, gemination, etc.), akin to how it's used in Synthesizer V);
### Other features:
- This model makes use of the [PC-NSF-HiFiGAN vocoder](https://github.com/openvpi/vocoders/releases/tag/pc-nsf-hifigan-44.1k-hop512-128bin-2025.02), which has support for tone shift. This can be convenient in lieu of vocal modes and/or variance embeds.
- Trained on reflow, LYNXNet (acoustic), WaveNet (duration + pitch), RoPE.
- All dictionaries contain support for Japanese kana (both hiragana and katakana).
- The English dictionary has support for Korean Hangeul as well.
    - Please make sure to enter Korean lyrics phonetically rather than as-written when combining with English on the same track.
- The Japanese dictionary also contains support for romaji (Hepburn).
- The Korean dictionary also contains support for romaja (Revised Romanization).
### Additional notes
- The pitch model may not be perfect and may need multiple rendering attempts in order to get the desired result. However, it should be decently usable in most contexts.

## Attribution
### Datasets used for training
- [Opencpop](https://wenet.org.cn/opencpop) by Opencpop Team (CC BY-NC-ND 4.0)
- [Project AI❤dol Public English Dataset](https://github.com/lottev1991/Project-AIdol-Public-English-Dataset) by Lotte V (CC BY-NC-SA 4.0) (includes unreleased private data)
- [PJS Corpus](https://sites.google.com/site/shinnosuketakamichi/research-topics/pjs_corpus) by Shinnosuke Takamichi & Junya Koguchi (CC BY-SA 4.0)
- [nitech_jp_song070_f001](https://hts.sp.nitech.ac.jp) by HTS Working Group (CC BY 3.0) 
- [CSD (Children's Song Dataset)](https://zenodo.org/records/4785016) (partial Korean data only) by KAIST Music and Audio Computing Lab (CC BY-NC-SA 4.0)

### Additional attributions
- Opencpop relabel by: [komisteng](https://github.com/komisteng) (https://huggingface.co/komisteng)
    - Pitch extraction, additional fixes by: [Lotte V](https://github.com/lottev1991) (https://lottev.moe)
- PJS relabel by: [UtaUtaUtau](https://github.com/UtaUtaUtau/pjs-manual-labels) (CC BY-SA 4.0)
- Partial CSD relabel by: [heta-tan](https://drive.google.com/file/d/1loh3AYkHoiyty0SW642kqE6-h4mRuchy/view?usp=sharing)
- Original project icon by: [Desti Silvana Ekasari](https://thenounproject.com/icon/mooncake-5021078) from The Noun Project (CC BY 3.0)
    - Color editing by: Lotte V
    - Please note that if you wish to reuse this icon, you should credit both creators listed above and link back to the Noun Project page.