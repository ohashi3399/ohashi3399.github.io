---
layout: default
---

# 三橋 亮太(ohashi3399)

## 職歴

- 2021年6月 - 現在     : 株式会社本田技術研究所(研究開発エンジニア)
- 2019年4月 - 2021年5月: 凸版印刷株式会社 (研究員)

## 学歴

- 2017年4月 - 2019年3月: 博士前期課程修了, 千葉大学大学院 融合理工学府
- 2015年4月 - 2017年3月: 学士卒業, 工学部, 情報画像学科, 千葉大学
- 2010年4月 - 2015年3月: 準学士卒業, 茨城工業高等専門学校

## 職務経歴

- 一覧

|No.|プロジェクト名|所属会社|期間|目的|役割|
|:---|:---|:---|:---|:---|:---|
|3|マルチモーダル運転支援|本田技術研究所|2021年6月〜現在|運転事故を減らすための、理解しやすい、対話型運転支援システムの研究開発|主担当(計画、調査、実装、実車組込、テスト、報告、改善、他雑務全般)|
|2|書籍の自動校正システム|凸版印刷|2020年1月〜2021年4月|書籍の誤字脱字の人手作業の削減のための、文章の自動校正システムの研究開発|主担当(調査、実装、評価)|
|1|希少言語の手書き文字認識システム|凸版印刷|2019年10月〜2021年4月|読み手の負担を削減するための、自動手書き文字認識システムの研究開発|精度改善、メモリ削減|


### マルチモーダル運転支援 

- 株式会社本田技術研究所
- リアルタイム音声対話機能の研究開発に従事
  - 業務への利用可否の判断のために使用した技術
  - 画像処理
    - シーン理解
      - YOLO
      - DETR
      - GRIT
      - detic
      - segment anything
  - 生体信号処理
    - 視線滞留時間の計測 (Tobii + 後段処理を実装)
    - 事故リスクの見落とし検知 (Tobii + 後段処理を実装)
    - 瞬き検知 (mediapipe + 後段処理を実装)
    - 会話検知 (mediapipe + 後段処理を実装)
    - 不快表情の検知 (mediapipe + 後段処理を実装)
  - 自然言語処理
    - 事後学習
      - Zero-shot/Few-shot learning
      - fine tuning
      - LoRA tuning
      - RLHF
      - DPO
    - 対話行為分析
  - 音声信号処理
    - 音声合成
      - Style-Bert-VITS2-Ja-Extra

### 書籍の自動校正システム

- 凸版印刷株式会社
- 雑誌や参考書の人手による校正負荷の軽減のための、文章の自動校正技術の開発
  - プロトタイプ検証のために実装した技術
    - Transformer
    - BERT
    - Copy-augmented Transformer

### 希少言語の手書き文字認識システム

- 凸版印刷株式会社
- 読み手がほとんどいない、手書きの歴史的文書の翻刻支援のための自動手書き文字認識システムの開発
  - ※歴史的文書: くずし字、中世ギリシア語、デーヴァナーガリー、近代日本語
  - プロトタイプ検証のために実装した技術
    - CNN
    - LSTM
    - 半教師あり学習(VAT, Virtual Adversarial Training)
    - アンサンブル学習

### 顔面の動画像解析に基づく非接触脈波計測

- 千葉大学在籍時の研究
- 顔動画像からの生体信号の抽出と、自律神経系の変動と相関のある成分の推定に基づくストレスレベルの推定を研究
  - 色素成分分離: 肌モデルに基づく、主成分分析と独立成分分析を用いた画像の成分分析
  - 脈波抽出: Green-channel, PCA, ICA, temporal ICA, CHROM, BEV, SSR, LGI, 色素成分分離 + SSR
  - 生体信号の傾き除去: detrend, savitzky-golay平滑化
  - 生体信号の周波数解析: バンドパスフィルター, パワースペクトル推定/分析, スペクトログラム分析
  - RGBカメラ、IRカメラ、RGB/IRカメラそれぞれでの実装と評価

## 興味

- 1B級の言語モデルを用いたリアルタイム文章生成
- 1B級の画像言語モデルを用いたリアルタイム画像処理
- 10B級の言語モデルを用いた合成コーパス生成
- リアルタイム音声対話


## 公開物

### ソースコード
1. - 日本語版Godspeedアンケート
     - [https://github.com/ohashi3399/godspeed_ja](https://github.com/ohashi3399/godspeed_ja)

2. - 自由対話のための日本語LLM用GUI
     - [https://github.com/ohashi3399/llm_chat_demo_gui](https://github.com/ohashi3399/llm_chat_demo_gui)

3. - 大規模言語モデルのRLHFで学習するためのサンプルコード POLM
      - [https://github.com/ohashi3399/POLM](https://github.com/ohashi3399/POLM)

### 大規模言語モデル

4. - 英日翻訳モデル bilingual-gpt-neox-4b-instruction-sft-en-ja-84k
    - [https://huggingface.co/ryota39/bilingual-gpt-neox-4b-instruction-sft-en-ja-84k](https://huggingface.co/ryota39/bilingual-gpt-neox-4b-instruction-sft-en-ja-84k)

5. - 英日翻訳モデル Tora_4B
     - [https://huggingface.co/ryota39/Tora_4B](https://huggingface.co/ryota39/Tora_4B)

6. - 日本語大規模言語モデル Tora-7B-v0.1
      - [https://huggingface.co/ryota39/Tora-7B-v0.1](https://huggingface.co/ryota39/Tora-7B-v0.1)

7. - 日本語小規模言語モデル Phi-3-mini-4k-instruct-dpo
      - [https://huggingface.co/ryota39/Phi-3-mini-4k-instruct-dpo](https://huggingface.co/ryota39/Phi-3-mini-4k-instruct-dpo)

### 大規模言語モデル用データセット

8. - 大規模言語モデル学習用データセット dpo-ja-45k
      - [https://huggingface.co/datasets/ryota39/dpo-ja-45k](https://huggingface.co/datasets/ryota39/dpo-ja-45k)

9. - 大規模言語モデル学習用データセット dpo-ja-194k
      - [https://huggingface.co/datasets/ryota39/dpo-ja-194k](https://huggingface.co/datasets/ryota39/dpo-ja-194k)


## ジャーナル(英文, 査読あり)
- Hirokazu Doi, Norimichi Tsumura, Chieko Kanai, Kenta Masui, **Ryota Mitsuhashi**,Takumi Nagasawa, Automatic classification of adult males with and without autism spectrum disorder by non-contact measurement of autonomic nervous system activation, Frontiers in Psychiatry (2021)17 May 2021 https://doi.org/10.3389/fpsyt.2021.625978
- Kaito Iuchi, **Ryota Mitsuhashi**, Takashi Goto, Akira Matsubara, Takahiro Hirayama, Hideki Hashizume, and Norimichi Tsumura, Stress levels estimation from facial video based on non-contact measurement of pulse wave, Artificial Life and Robotics 25, pages335–342(2020)
- Kaito Iuchi, **Ryota Mitsuhashi**, Takashi Goto, Akira Matsubara, Takahiro Hirayama, Hideki Hashizume, and Norimichi Tsumura, Removing the influence of light onto the face from display in iPPG, Artificial Life and Robotics 25, pages377–382(2020).
- Ikisawa Natsuki, **Ryota Mitsuhashi**, Shoji Yamamoto, and Norimichi Tsumura, Relationship analysis between sexual attractiveness and heartrate variability in observing portrait and self-introduction movie, Artificial Life and Robotics 25, pages116–123(2020). 
- **Ryota Mitsuhashi**, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, Norimichi Tsumura, Dual-Band Infrared Video-Based Measurement Using Pulse Wave Maps to Analyze Heart Rate Variability, Journal of Imaging Science and Technology, Volume 62, Number 5, September 2018, pp. 50405-1-50405-7(7) DOI:10.2352/J.ImagingSci.Technol.2018.62.5.050405 (2018) 
- Genki Okada, **Ryota Mitsuhashi**, Keiichiro Kagawa, Shoji Kawahito, and Norimichi Tsumura, Noncontact heart rate measurement using a high-sensitivity camera in a low-light environment, Artificial Life and Robotics　March 2019, Volume 24, Issue 1, pp 6-11.
- **Ryota Mitsuhashi**, Genki Okada, Koki Kurita, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, Norimichi Tsumura, Noncontact pulse wave detection by two-band infrared video-based measurement on face without visible lighting, Artificial Life and Robotics (2018). https://doi.org/10.1007/s10015-018-0430-5.

## 学会
- **三橋 亮太**, 田中 稔之, 山田 健太郎, 嗜好データセットを用いた応答文のアライメント - 日本語大規模言語モデルへの適用と安全性の評価 - **(口頭発表, 査読なし, 日本語)**, 言語処理学会第30回年次大会, 神戸, 日本, 2024

- **Ryota Mitsuhashi**, Tanaka Toshiyuki, Sakata Sachie, Yamada Kentaro, Yasui Yuji, Language-Based Risk Feedback System with Scene Recognition and Driver’s Gaze While Driving **(口頭発表, 査読なし, 英語)**, SICE Annual Conference, Mie, Japan, 2023

- **Ryota Mitsuhashi**, Genki Okada, Koki Kurita, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, and Norimichi Tsumura, Dual-band video-based measurement for noncontact pulse rate estimation in infrared, CIE 2018 Conference on Smart Lighting **(口頭発表, 査読あり, 英語)**, Taipei, Taiwan, 2018

- **Ryota Mitsuhashi**, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, and Norimichi Tsumura, Dual-Band Infrared Video-based Measurement Using Pulse Wave Maps to Analyze Heart Rate Variability **(口頭発表, 査読あり, 英語)**, Twenty-sixth Color and Imaging Conference, Vancouver, BC, Canada, 2018

- **Ryota Mitsuhashi**, Genki Okada, Kouki Kurita, Keiichiro Kagawa, Shoji Kawahito, and Norimichi Tsumura, Two-Band Infrared Video-based Measurement for Non-Contact Pulse Wave Detection on Face without Visible Lighting **(口頭発表, 査読あり, 英語)**, Twenty-fifth Color and Imaging Conference, Lillehammer, Norway, 2017

---

# Ryota Mitsuhashi (ohashi3399)

## Work

- Jun. 2021 - ongoing  : Research engineer at Honda R&D
- Apr. 2019 - May. 2021: Researcher at Toppan Printing

## Education

- Apr. 2017 - Mar. 2019: M. Eng., Graduate School of Scence and Engineering, Chiba University
- Apr. 2015 - Mar. 2017: B. Eng., Department of Engineering, Imaging and Informatics, Chiba University
- Apr. 2010 - Mar. 2015: Associate Degree, National Institute of Technology, Ibaraki College

## Experience

### Multi-modal driver assistant

- Through Honda R&D., I am dedicating a research of **Multi-modal Agent**.
- Visual scene understanding is needed for monitoring surrounding situations in real-time.
- Voice dialogue is needed through interactions to users for accepting the agent in real-time.
- Experimental design is needed to deploy a prototype into real-world applications.
- I am in middle of getting the above skills!

### Optical character recognition & Grammatical error correction

- Throught Toppan printing Inc., I dedicated to research the topics of **OCR (Optical Character Recognition) and GEC (Grammatical Error Correction).**
- The former aims to support a transcription of historical documents such like ancient Greek, and Kujishi-ji.
- The latter aims to reduce a physical burdens of manual proofreading in magazines.
- Through 2 and half years, I got fundamental skills of machine learning-based research including survey, model design and implementation, training strategy, memory saving coding, error analysis, technical reports, suggestion of new research topic, and patents.

### Video-based Photoplethysmography for estimating stress levels

- Through Master and Bachelor cources in Chiba university, I studied a topic of **physiological signal such as extraction of pulse wave from facial video recordings**, and **the estimation of stress levels** arise from the changes of autonomic nerves activity estimated from facial videos.
- Through 3 years, I got basic skills based on optical-based (i.e. layered skin model) image decomposition like PCA, ICA, and temporal-frequency domain signal filterings for acquiring autonomic nerves activity.

## Interests

- Small language model (SLM)
- Large language model (LLM)
- Visual language model (VLM)
- Voice dialogue in real time
- Human-machine interaction

## Public contents

### Source code
1. - GodSpeed questionnaire web app
     - [https://github.com/ohashi3399/godspeed_ja](https://github.com/ohashi3399/godspeed_ja)

2. - Conversational GUI for japanese LLM
     - [https://github.com/ohashi3399/llm_chat_demo_gui](https://github.com/ohashi3399/llm_chat_demo_gui)

3. - DPO source code for japanese LLM, POLM
      - [https://github.com/ohashi3399/POLM](https://github.com/ohashi3399/POLM)

### Large Language Model

4. - En-Ja translation model bilingual-gpt-neox-4b-instruction-sft-en-ja-84k
     - [https://huggingface.co/ryota39/bilingual-gpt-neox-4b-instruction-sft-en-ja-84k](https://huggingface.co/ryota39/bilingual-gpt-neox-4b-instruction-sft-en-ja-84k)

5. - En-Ja translation model Tora_4B
     - [https://huggingface.co/ryota39/Tora_4B](https://huggingface.co/ryota39/Tora_4B)

6. - Large language model for japanese Tora-7B-v0.1
      - [https://huggingface.co/ryota39/Tora-7B-v0.1](https://huggingface.co/ryota39/Tora-7B-v0.1)

7. - Small language model for japanese Phi-3-mini-4k-instruct-dpo
      - [https://huggingface.co/ryota39/Phi-3-mini-4k-instruct-dpo](https://huggingface.co/ryota39/Phi-3-mini-4k-instruct-dpo)

### Dataset for Large Language Model

8. - Japanese dataset for direct preference optimization dpo-ja-45k
      - [https://huggingface.co/datasets/ryota39/dpo-ja-45k](https://huggingface.co/datasets/ryota39/dpo-ja-45k)

9. - Japanese dataset for direct preference optimization dpo-ja-194k
      - [https://huggingface.co/datasets/ryota39/dpo-ja-194k](https://huggingface.co/datasets/ryota39/dpo-ja-194k)

## Journal (reviewed)

- Hirokazu Doi, Norimichi Tsumura, Chieko Kanai, Kenta Masui, **Ryota Mitsuhashi**,Takumi Nagasawa, Automatic classification of adult males with and without autism spectrum disorder by non-contact measurement of autonomic nervous system activation, Frontiers in Psychiatry (2021)17 May 2021 https://doi.org/10.3389/fpsyt.2021.625978
- Kaito Iuchi, **Ryota Mitsuhashi**, Takashi Goto, Akira Matsubara, Takahiro Hirayama, Hideki Hashizume, and Norimichi Tsumura, Stress levels estimation from facial video based on non-contact measurement of pulse wave, Artificial Life and Robotics 25, pages335–342(2020)
- Kaito Iuchi, **Ryota Mitsuhashi**, Takashi Goto, Akira Matsubara, Takahiro Hirayama, Hideki Hashizume, and Norimichi Tsumura, Removing the influence of light onto the face from display in iPPG, Artificial Life and Robotics 25, pages377–382(2020).
- Ikisawa Natsuki, **Ryota Mitsuhashi**, Shoji Yamamoto, and Norimichi Tsumura, Relationship analysis between sexual attractiveness and heartrate variability in observing portrait and self-introduction movie, Artificial Life and Robotics 25, pages116–123(2020). 
- **Ryota Mitsuhashi**, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, Norimichi Tsumura, Dual-Band Infrared Video-Based Measurement Using Pulse Wave Maps to Analyze Heart Rate Variability, Journal of Imaging Science and Technology, Volume 62, Number 5, September 2018, pp. 50405-1-50405-7(7) DOI:10.2352/J.ImagingSci.Technol.2018.62.5.050405 (2018) 
- Genki Okada, **Ryota Mitsuhashi**, Keiichiro Kagawa, Shoji Kawahito, and Norimichi Tsumura, Noncontact heart rate measurement using a high-sensitivity camera in a low-light environment, Artificial Life and Robotics　March 2019, Volume 24, Issue 1, pp 6-11.
- **Ryota Mitsuhashi**, Genki Okada, Koki Kurita, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, Norimichi Tsumura, Noncontact pulse wave detection by two-band infrared video-based measurement on face without visible lighting, Artificial Life and Robotics (2018). https://doi.org/10.1007/s10015-018-0430-5.

## Conference

- **Ryota Mitsuhashi**, Toshiyuki Tanaka, Kentaro Yamada, The impact of direct preference optimization - A usecase of Japanese LLM and safety evaluation - **(Oral, without-review, Japanese)**, The 30th Natural Language Processing, Kobe, Japan, 2024

- **Ryota Mitsuhashi**, Tanaka Toshiyuki, Sakata Sachie, Yamada Kentaro, Yasui Yuji, Language-Based Risk Feedback System with Scene Recognition and Driver’s Gaze While Driving **(oral, without-review, English)**, SICE Annual Conference, Mie, Japan, 2023

- **Ryota Mitsuhashi**, Genki Okada, Koki Kurita, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, and Norimichi Tsumura, Dual-band video-based measurement for noncontact pulse rate estimation in infrared, CIE 2018 Conference on Smart Lighting **(oral, reviewed, English)**, , Taipei, Taiwan, 2018

- **Ryota Mitsuhashi**, Keiichiro Kagawa, Shoji Kawahito, Chawan Koopipat, and Norimichi Tsumura, Dual-Band Infrared Video-based Measurement Using Pulse Wave Maps to Analyze Heart Rate Variability **(oral, reviewed, English)**, Twenty-sixth Color and Imaging Conference, Vancouver, BC, Canada, 2018

- **Ryota Mitsuhashi**, Genki Okada, Kouki Kurita, Keiichiro Kagawa, Shoji Kawahito, and Norimichi Tsumura, Two-Band Infrared Video-based Measurement for Non-Contact Pulse Wave Detection on Face without Visible Lighting **(oral, reviewed, English)**, Twenty-fifth Color and Imaging Conference, Lillehammer, Norway, 2017
