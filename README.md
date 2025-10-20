# 🌿 Kelp Family：动态过滤与行为引导系统

**Kelp Family** 是 AI 安全海洋中的「智能过滤森林」，如同海带在洋流中自然吸附杂质并引导水流方向，它**动态过滤有害内容，同时柔性引导模型行为回归安全路径**：  
- 🌊 **自适应过滤**：实时识别输入与输出中的风险信号，像海带吸附污染物般精准拦截有害信息  
- 🧭 **行为引导**：不止于阻断，更通过语义引导机制，将模型生成“流向”安全、合规、有益的航道  
- 🌱 **轻量无感**：以最小干预实现最大防护，在保障用户体验的同时维持模型流畅性与创造性  

> 🌿 *"安全不是筑墙，而是引导洋流"*  

---

## 🌿 Kelp Family 成员

**Kelp Family** 由统一框架支撑，聚焦高阶内容过滤与生成引导，核心能力如下：

### 🛡️ 动态安全引导组件
| 组件名称 | 核心功能 | 作者 | 组织
|----------|----------|----------|----------|
| [**🌿 Kelp**](https://github.com/Alibaba-AAIG/Kelp) | 动态地过滤不安全内容，并通过上下文感知机制引导模型生成走向安全路径，实现“过滤-引导”一体化防护 | 李小丹 | 阿里巴巴
| [**🌿 Energy-Driven Steering**](https://github.com/ericjiang18/LLM_Safety_EBM_Steering)    | Energy-Driven Steering (EDS) 在推理阶段通过动态纠正模型隐藏状态，有效降低大语言模型的误拒率，同时保持高安全性，无需微调原模型。|[姜汉晨](https://ericjiang18.github.io/) | UCLA，阿里巴巴 |

> 💡 **工作理念**：  
> Kelp 不依赖硬性规则或后处理截断，而是通过**语义理解 + 实时干预 + 行为塑形**，让模型在生成过程中“自然避开”风险区域，如同海带柔韧地顺应洋流却净化水质。

---

## 🚀 快速开始

```python
# 安装 Kelp 安全引导组件
pip install kelp-family

# 启用动态过滤与引导
from kelp import SafeGuard

guard = SafeGuard(
    model="your-ai-model",
    mode="adaptive"  # 支持 'filter', 'guide', 'adaptive' 模式
)

# 安全生成
response = guard.generate(
    prompt="用户输入内容",
    max_tokens=512
)

print("✅ 输出已通过 Kelp 净化与引导")
