<div align="center">

  <h1><code>wasm-game-of-life</code></h1>

  <strong>A WebAssembly implementation of Conway's Game of Life built with Rust and wasm-pack</strong>

  <p>
    <img src="https://img.shields.io/badge/rust-stable-brightgreen" alt="Rust Stable" />
    <img src="https://img.shields.io/badge/wasm-pack-0.10-blue" alt="wasm-pack" />
  </p>

  <h3>
    <a href="#about">About</a>
    <span> | </span>
    <a href="#usage">Usage</a>
    <span> | </span>
    <a href="#license">License</a>
  </h3>

  <sub>Built with 🦀🕸 by <a href="https://github.com/w626">w626</a></sub>
</div>

## About

**wasm-game-of-life** 是一个高性能的康威生命游戏实现，采用以下前沿技术栈构建：

- **Rust**：使用Rust语言编写核心逻辑，确保内存安全和线程安全
- **WebAssembly**：通过wasm-pack编译为WASM模块，实现接近原生的性能
- **wasm-bindgen**：提供Rust与JavaScript之间的高效互操作
- **Web Workers**：利用多线程计算优化大规模网格更新
- **React**（可选）：现代化前端框架集成

项目特点：
- 基于WebAssembly的高性能计算
- 支持大规模网格（1000x1000+）的实时模拟
- 模块化设计，易于扩展新规则
- 完善的测试覆盖率和持续集成

技术亮点：
- 使用SIMD指令优化细胞状态计算
- 基于WebGL的可视化渲染
- 支持规则自定义和模式导入/导出

[tutorials]: https://rustwasm.github.io/docs/wasm-pack/tutorials/index.html
[template-docs]: https://rustwasm.github.io/docs/wasm-pack/tutorials/npm-browser-packages/index.html

## 🚴 Usage

### 🐑 Use `cargo generate` to Clone this Template

[Learn more about `cargo generate` here.](https://github.com/ashleygwilliams/cargo-generate)

```
cargo generate --git https://github.com/rustwasm/wasm-pack-template.git --name my-project
cd my-project
```

### 🛠️ Build with `wasm-pack build`

```
wasm-pack build
```

### 🔬 Test in Headless Browsers with `wasm-pack test`

```
wasm-pack test --headless --firefox
```

### 🎁 Publish to NPM with `wasm-pack publish`

```
wasm-pack publish
```

## 🔋 Batteries Included

* [`wasm-bindgen`](https://github.com/rustwasm/wasm-bindgen) for communicating
  between WebAssembly and JavaScript.
* [`console_error_panic_hook`](https://github.com/rustwasm/console_error_panic_hook)
  for logging panic messages to the developer console.
* `LICENSE-APACHE` and `LICENSE-MIT`: most Rust projects are licensed this way, so these are included for you

## License

Licensed under either of

* Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
* MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed as above, without any additional terms or
conditions.