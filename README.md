## 概要

**PoseAudioInteraction**は、Mediapipeを用いた姿勢推定に基づき、ユーザーの体の動きに応じて立体音響を制御するシステムの予定。ユーザーが音源に近づくと音が大きくなり、遠ざかると音が小さくなる動的な音響環境を提供。

## 特徴

- **リアルタイム姿勢推定**: Mediapipeを使用して、ユーザーの体のキーポイントをリアルタイムで検出
- **動的音響制御**: ユーザーの体の位置に基づいて音量を動的に調整
- **インタラクティブな3D音響環境**: 音源がユーザーの動きに適応して、よりリアルな立体音響を提供

## 使用技術

- **Unity**: 3D環境と音響制御のために使用
- **Mediapipe**: リアルタイム姿勢推定のために使用
- **C#**: Unityスクリプトの記述に使用
- **Native WebSocket**: WebSocket通信を利用してリアルタイムデータを送受信し、音響制御や姿勢推定のデータを同期

## クローン手順

このプロジェクトにはサブモジューを含んでいる為、リポジトリをクローンした後、以下のコマンドを実行してサブモジュールを初期化し、必要な依存関係を取得する必要あり。

```bash
git clone https://github.com/ISSE0116/PoseAudioInteraction.git 
cd https://github.com/ISSE0116/PoseAudioInteraction.git
git submodule update --init --recursive

