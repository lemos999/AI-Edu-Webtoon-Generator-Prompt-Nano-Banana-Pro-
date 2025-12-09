# 🎨 AI Edu-Webtoon Generator (Nano Banana Pro)

An educational webtoon generation prompt system optimized for the **Nano Banana Pro** model.
It leverages multimodal capabilities to function as a consistent **Serialized Manga Agent**, going beyond simple image generation.

## 📌 Core Features

*   **8-Panel Vertical Webtoon:** Optimized for mobile scrolling (1:3~1:4 aspect ratio).
*   **Variable Meta-Layout:** Randomizes panel compositions (Wide, Split, Tall, Diagonal) for every episode to prevent visual fatigue.
*   **Character Persistence (Vision Protocol):** Analyzes attached user images to extract and lock visual traits (DNA), ensuring character consistency across all episodes.
*   **Socratic Pacing:** Breaks topics into micro-steps. The final panel always ends with a **leading question** to stimulate metacognition and trigger the next episode.
*   **Clean Rendering:** Implements strictly isolated logic to prevent prompt meta-instructions from leaking into speech bubbles.

## 🚀 Usage

### 1. Installation
Copy and paste the entire provided `System Prompt` into the **Nano Banana Pro** model context.

### 2. Triggers
Control the generation using the following keywords:

| Trigger | Function | Behavior |
| :--- | :--- | :--- |
| **"Draw [Topic]"** | Create Ep.1 | Generates an 8-panel webtoon covering the basics (Default persona applied). |
| **(Attach Image)** | Set Character | Instantly analyzes the image and locks it as the main character. |
| **"Continue" / "Next"** | Create Next Ep. | Generates the next logical step based on previous context (Layout changes automatically). |

## 🛠️ Technical Logic

The system executes the following 4-step protocol sequentially:

1.  **Vision Analysis:** Checks for image attachments and updates Character DNA.
2.  **Layout Randomization:** Diversifies the grid structure for panels 2-7.
3.  **Payload Construction:** Assembles the specialized English prompt for Nano Banana Pro.
4.  **Execution:** Immediately calls the image generation tool and renders Korean dialogue.


---

# 🎨 AI Edu-Webtoon Generator (Nano Banana Pro)

**Nano Banana Pro** 모델의 멀티모달(Vision & Image Generation) 능력을 극대화한 **교육용 연재 웹툰 생성 프롬프트 시스템**입니다.
단순한 이미지 생성을 넘어, 연속성을 가진 **만화 작가 에이전트**를 구현합니다.

## 📌 핵심 기능 

*   **8-Panel Vertical Webtoon:** 모바일 환경에 최적화된 8컷 세로 스크롤 웹툰 포맷 (1:3~1:4 비율).
*   **Variable Meta-Layout:** 매 에피소드마다 컷 배치(Wide, Split, Tall, Diagonal)를 무작위로 변형하여 시각적 피로도 방지.
*   **Character Persistence (Vision Protocol):** 사용자가 첨부한 이미지의 시각적 특징(DNA)을 추출 및 저장하여 전 에피소드에 걸쳐 캐릭터 일관성 유지.
*   **Socratic Pacing:** 주제를 한 번에 끝내지 않고 '마이크로 단위'로 쪼개어 설명하며, 마지막 컷은 반드시 **질문**을 던져 학습을 유도.
*   **Clean Rendering:** 프롬프트 명령어(Meta-text)가 말풍선에 누수되는 현상을 완벽 차단하는 격리 로직 적용.

## 🚀 사용 방법 

### 1. 시스템 프롬프트 적용 
제공된 `System Prompt` 전체를 **Nano Banana Pro** 모델의 시스템 설정(또는 첫 대화)에 입력합니다.

### 2. 트리거 명령어 
채팅창에 다음 키워드를 사용하여 웹툰 생성을 제어합니다.

| 명령어 | 기능 | 동작 방식 |
| :--- | :--- | :--- |
| **"[주제] 그려"** | 1화 생성 | 주제의 가장 기초 개념을 8컷 웹툰으로 생성 (기본 캐릭터 적용) |
| **(이미지 첨부)** | 캐릭터 변경 | 첨부된 이미지의 특징을 즉시 분석하여 새로운 주인공으로 고정 |
| **"계속 그려"** | 다음 화 연재 | 이전 질문에 대한 답을 기반으로 심화 과정 생성 (레이아웃 자동 변경) |

## 🛠️ 기술적 로직 

이 시스템은 다음 4단계 프로토콜을 순차적으로 실행합니다.

1.  **Vision Analysis:** 첨부 이미지 유무 확인 및 캐릭터 DNA 추출.
2.  **Layout Randomization:** 2~7번 컷의 레이아웃 구조 가변 생성.
3.  **Payload Construction:** Nano Banana Pro 전용 영문 프롬프트(Payload) 조립.
4.  **Execution:** 이미지 생성 도구 즉시 호출 및 한국어 대사 렌더링.

## 📜 License
MIT License

---
