# deploy_jd359

**追溯模型部署工程师·结构化输出的约束解码里每一份贡献来自哪里。**

`deploy_jd359` —— 统计各来源片段的贡献量与占比，标出模型部署工程师·结构化输出的约束解码上最主要的来源

- 零依赖，Python 3.10+ 标准库即可运行
- 单文件，`deploy_jd359.py` 拷走就能用
- 不联网、不写文件

## 对应的岗位

- 目标岗位：**小米 · 负责人模型部署工程师**
- 技能主线：MLOps、Docker、Kubernetes、大模型推理
- 领域标签：MLOps、AI基础设施
- 研究方向：模型部署工程师·结构化输出的约束解码

工具里的规则表就是照着上面这条岗位要求建的——每条规则都挂在技能线或领域标签上，命中时能指回具体要求。

<!-- ipos:install -->
## 安装

零依赖，Python 3.10+ 即可：

```bash
pip install webin88-deploy_jd359
```

装完直接用命令名调用：

```bash
deploy_jd359 --help
```

也可以不用安装，直接把 `deploy_jd359.py` 拷走用——它只依赖标准库。

## 为什么需要它

贡献占比按字符量算而不是按出现次数，避免长句主导统计

它遵守下面几条自己定的规矩：

1. **只报告能定位到具体位置的结论**，不做语义猜测。
2. **规则表公开**，每条命中都能对应到岗位要求的一条明示规则。
3. **输入为空或格式不对时明确报错**，不静默返回空结果。

## 用法

```bash
python deploy_jd359.py --file input.txt
python deploy_jd359.py --text "示例内容"
python deploy_jd359.py --file input.txt --json
```

加 `--json` 可以拿到机器可读的结果，便于接到流水线里。

## 已知局限

- 计数按字面 token 统计，不做词形还原。
- 只报告分布，不判断该保留哪些。

## 跑测试

```bash
python test_deploy_jd359.py
```

测试用独立的断言与临时数据，不污染工作目录。

## 来源与参考

- Python 标准库文档：<https://docs.python.org/3/>
- GitHub 仓库：<https://github.com/webin88/deploy_jd359>

---

## 关于作者

webin88 做模型部署工程师·结构化输出的约束解码相关的问题，方向对标小米的负责人模型部署工程师岗位。这个工具先替你回答一个具体问题，再谈别的。

- 个人主页：<https://webin88.github.io>
- 仓库：<https://github.com/webin88/deploy_jd359>

## 许可

MIT，见 [LICENSE](LICENSE)。
