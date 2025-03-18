# ShadowPulse

ShadowPulse は、低レイヤーのネットワーク制御を学習するために開発されたDDoSシミュレーションツール。  
ネットワークの動作や防御対策を理解し、セキュリティに関する知識を深めることを目的としている。

## 特徴
- Windows環境向けのDDoSテストツール
- 低レイヤーのネットワークプログラミングを活用（Raw Socket, WinSock, Npcap）
- **SYN Flood / UDP Flood / ICMP Flood / HTTP Flood** を実装予定
- **防御策（レートリミット, WAF, ファイアウォール）** も検証可能

---

## 技術スタック
- **言語:** C++, Rust
- **ネットワークAPI:** WinSock, Npcap
- **監視ツール:** Wireshark, Windows Firewall API

---

## セットアップ
### 1. 必要なツールのインストール
1. [Visual Studio](https://visualstudio.microsoft.com/)（C++ 開発環境）
2. [Npcap](https://nmap.org/npcap/)（パケットキャプチャ用）
3. [Wireshark](https://www.wireshark.org/)（ネットワーク監視）

### 2. プロジェクトのクローン
```
git clone https://gitlab.com/your_username/ShadowPulse.git cd ShadowPulse
```

### 3. ビルド
Visual Studioでプロジェクトを開き、管理者権限でビルドする。

---

## 実装予定の機能
- [x] **ICMP Flood**（Ping連続送信）
- [ ] **SYN Flood**（TCP SYNパケットを大量送信）
- [ ] **UDP Flood**（UDPパケットを送信し続ける）
- [ ] **HTTP Flood**（Webサーバーへのリクエスト攻撃）
- [ ] **DDoS防御策のシミュレーション**（レートリミット, WAF設定）

---

## 免責事項
このプロジェクトは **教育目的の研究開発** を目的としたものであり、  
**実際の攻撃や不正アクセスには絶対に使用しないこと。**  
本ツールを使用したことによるいかなる損害・責任も負わない。

---

## ライセンス
MIT License
