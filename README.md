<h1 align="center">The Spica Compiler Platform</h1>

**EN**

> ⚠️ **Notice**
> 
> * **This repository is an unofficial fork of [.NET Compiler Platform (Roslyn)](https://github.com/dotnet/roslyn).** It is not affiliated with or endorsed by Microsoft.
> * **Work in Progress:** This project is currently incomplete and does not contain any custom modifications yet.
> * If you are looking for the official code or standard releases, please visit and download directly from the **[Official Roslyn Repository](https://github.com/dotnet/roslyn)**.

---

### Credits & License

* **Original Project:** [.NET Compiler Platform (Roslyn)](https://github.com/dotnet/roslyn)
* **Copyright:** Copyright (c) Microsoft Corporation. All rights reserved.
* **License:** Licensed under the [MIT License](https://github.com/dotnet/roslyn/blob/main/License.txt).

### Project Goals & Vision

**"Achieving memory management flexibility comparable to C++ while retaining C#'s refined syntax and ease of writing."**

This project (Spica) aims to build a fully controlled C# language platform—free from the constraints of Garbage Collection (GC)—by extending and experimenting with the Roslyn compiler infrastructure.

#### Planned Features

1. **Elimination of Garbage Collection (GC)**
   * Eliminate "Stop-the-World" pauses and unpredictable latency caused by GC.
   * Ensure deterministic behavior optimized for real-time systems, game engines, and low-latency processing.

2. **C++-Level Memory Management Flexibility**
   * Enable explicit memory allocation and deallocation by the developer (e.g., `new`/`delete` or custom allocators).
   * Integrate concepts like ownership models (RAII) and smart pointers at the compiler level to allow flexible pointer manipulation and heap management.

3. **Zero-Cost Abstractions and Native Performance**
   * Leverage C# classes and powerful language features while generating native code that incurs absolutely no unnecessary internal overhead.

> 💡 *We are currently in the verification and preparation phase for the Roslyn infrastructure. We will proceed incrementally with syntax extensions and the implementation of static analysis features.*

As for whether I can actually complete this—I can't say "no," but I can't say "yes" either. I've been busy lately, so I apologize in advance if the project ends up being scrapped.


---

### .NET Foundation

This project incorporates code originally developed as part of the [.NET Foundation](http://www.dotnetfoundation.org/projects) along with other projects like [the .NET Runtime](https://github.com/dotnet/runtime/).




**JP**

> **注意**
> 
> * **本リポジトリは [.NET Compiler Platform (Roslyn)](https://github.com/dotnet/roslyn) の非公式（Unofficial）フォークです。** Microsoft 公式のプロジェクトではなく、提携・承認されたものでもありません。
> * **現在開発中（未完成）:** 本プロジェクトは現在作業中であり、現時点では独自のカスタマイズや変更は含まれていません。
> * 公式のコードや標準リリースをお探しの場合は、**[Microsoft 公式の Roslyn リポジトリ](https://github.com/dotnet/roslyn)** から直接ダウンロード・ご利用いただくようお願いいたします。

---

### クレジット & ライセンス

* **オリジナルプロジェクト:** [.NET Compiler Platform (Roslyn)](https://github.com/dotnet/roslyn)
* **著作権表示:** Copyright (c) Microsoft Corporation. All rights reserved.
* **ライセンス:** [MIT License](https://github.com/dotnet/roslyn/blob/main/License.txt) に基づいて提供されています。


###プロジェクトの目的と最終目標 (Goals & Vision)

**「C# の洗練された構文・書きやすさを保ちながら、C++ と同等のメモリ管理自由度を実現する」**

本プロジェクト（Spica）は、Roslyn コンパイラ基盤を拡張・実験し、ガベージコレクション（GC）の制約を受けない完全制御型の C# 言語基盤の構築を目指しています。

#### 核心機能 (Planned Features)

1. **ガベージコレクション（GC）の撤去**
   * GC による一時停止（Stop-the-World）や不確実な遅延を排除。
   * リアルタイムシステムやゲームエンジン、低レイテンシ処理に特化した決定論的な動作。

2. **C++ 同等の自由なメモリ管理**
   * 開発者自身による明示的なメモリ確保・解放（`new` / `delete` やカスタムアロケータの利用）。
   * 所有権モデル（RAII）やスマートポインタ相当の概念をコンパイラレベルで組み込み、ポインタ操作やヒープ管理を柔軟に。

3. **ゼロコスト抽象化とネイティブパフォーマンス**
   * C# のクラスや強力な言語機能を活かしつつ、内部では不要なオーバーヘッドを一切生まないネイティブコード生成。

> 💡 *現在は Roslyn 基盤の確認・準備段階です。段階的に文法拡張および静的解析機能の実装を進めていきます。*
完成できるかも最近忙しいので没になったらすみません。
>
> ---

### .NET Foundation

本プロジェクトには、[the .NET Runtime](https://github.com/dotnet/runtime/) などのプロジェクトとともに、[.NET Foundation](http://www.dotnetfoundation.org/projects) の一環として元々開発されたコードが含まれています。
