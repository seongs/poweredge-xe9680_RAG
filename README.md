# xe9680_rag README

## 개요

xe9680_rag는 Dell Generative AI 예제 레포지토리에서 제공하는 기존 RAG 챗봇의 향상된 버전입니다. 이 노트북은 더 나은 기능성과 사용자 경험을 위해 몇 가지 새로운 기능과 개선 사항을 포함하고 있습니다.

## 주요 개선 사항

1. **모델 업데이트**: 기본 모델을 [mistralai/Mistral-7B-Instruct-v0.2](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)를 사용하고, poweredge-xe9680-technical-guide.pdf에서 파생된 한국어 데이터셋을 QLoRA를 사용하여 파인튜닝 했습니다.
2. **Gradio 통합**: 기존 버전은 미리 정의된 경로의 PDF를 참조했으나, 이 버전에서는 Gradio의 파일 업로드 기능을 추가하여 사용자가 원하는 PDF 문서를 업로드하고 이를 참조하여 질의에 응답할 수 있도록 했습니다.
3. **코사인 유사도 기능**: 참조 문서의 코사인 유사도를 계산하고 표시하여, 질의에 대한 문서의 관련성을 사용자에게 제공합니다.


## 라이선스
이 프로젝트는 MIT 라이선스에 따라 라이선스가 부여됩니다.

## 감사의 말
Dell의 원본 RAG 챗봇 예제에 감사드립니다.

인터페이스를 제공해준 Gradio에 감사드립니다.

[참고한 Dell Generative AI 예제](https://github.com/dell-examples/generative-ai/blob/main/RAG-chatbot-multiformat/rag-chatbot-multiformat-source-tabs.ipynb)
