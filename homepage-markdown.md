<style>
.na-home {
    --primary: #3B82F6;
    --primary-glow: rgba(59, 130, 246, 0.5);
    --secondary: #8B5CF6;
    --accent: #06B6D4;
    --success: #10B981;
    --bg-dark: #0f172a;
    --bg-card: rgba(30, 41, 59, 0.8);
    --text-primary: #F8FAFC;
    --text-secondary: #94A3B8;
    --border: rgba(148, 163, 184, 0.2);
    --gradient-main: linear-gradient(135deg, #3B82F6 0%, #8B5CF6 50%, #06B6D4 100%);
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    color: var(--text-primary);
    padding: 2rem;
    max-width: 1100px;
    margin: 0 auto;
}
.na-hero { text-align: center; padding: 2rem 0 3rem; }
.na-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: linear-gradient(135deg, rgba(59, 130, 246, 0.15) 0%, rgba(139, 92, 246, 0.15) 100%);
    border: 1px solid rgba(59, 130, 246, 0.3);
    border-radius: 50px;
    padding: 0.5rem 1.2rem;
    font-size: 0.9rem;
    color: var(--text-secondary);
    margin-bottom: 1.5rem;
}
.na-badge-dot {
    width: 8px;
    height: 8px;
    background: var(--success);
    border-radius: 50%;
    display: inline-block;
    animation: na-pulse 2s infinite;
}
@keyframes na-pulse {
    0%, 100% { opacity: 1; box-shadow: 0 0 10px var(--success); }
    50% { opacity: 0.5; box-shadow: 0 0 20px var(--success); }
}
.na-title {
    font-size: clamp(2rem, 5vw, 3rem);
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 1rem;
    background: var(--gradient-main);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
.na-desc {
    font-size: 1.1rem;
    color: var(--text-secondary);
    max-width: 600px;
    margin: 0 auto 2rem;
    line-height: 1.7;
}
.na-desc strong { color: var(--text-primary); }
.na-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
}
.na-btn {
    padding: 0.8rem 1.5rem;
    border-radius: 10px;
    font-size: 0.95rem;
    font-weight: 600;
    text-decoration: none;
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    transition: all 0.25s ease;
}
.na-btn-primary {
    background: linear-gradient(135deg, #3B82F6 0%, #2563EB 100%);
    color: #fff;
    box-shadow: 0 4px 15px var(--primary-glow);
}
.na-btn-primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 25px var(--primary-glow);
    color: #fff;
}
.na-btn-secondary {
    background: rgba(255, 255, 255, 0.05);
    color: var(--text-primary);
    border: 1px solid var(--border);
}
.na-btn-secondary:hover {
    background: rgba(59, 130, 246, 0.1);
    border-color: rgba(59, 130, 246, 0.3);
    transform: translateY(-2px);
}
.na-stats {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
    gap: 1rem;
    padding: 2rem 0;
}
.na-stat {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 1.5rem 1rem;
    text-align: center;
    transition: all 0.3s ease;
}
.na-stat:hover {
    border-color: rgba(59, 130, 246, 0.4);
    transform: translateY(-3px);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
}
.na-stat-value {
    font-size: 2rem;
    font-weight: 700;
    background: var(--gradient-main);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 0.3rem;
}
.na-stat-label {
    color: var(--text-secondary);
    font-size: 0.9rem;
}
.na-section { padding: 2rem 0; }
.na-section-title {
    text-align: center;
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    background: linear-gradient(180deg, var(--text-primary) 0%, var(--text-secondary) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
.na-section-desc {
    text-align: center;
    color: var(--text-secondary);
    margin-bottom: 2rem;
}
.na-models {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    justify-content: center;
}
.na-model {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 50px;
    padding: 0.5rem 1rem;
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    font-size: 0.9rem;
    transition: all 0.2s ease;
}
.na-model:hover {
    border-color: rgba(59, 130, 246, 0.4);
    transform: translateY(-2px);
}
.na-model-icon {
    width: 24px;
    height: 24px;
    border-radius: 6px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 700;
    font-size: 0.7rem;
    color: white;
}
.na-openai { background: #10A37F; }
.na-claude { background: #D97757; }
.na-gemini { background: #4285F4; }
.na-llama { background: #7C3AED; }
.na-mistral { background: #FF7000; }
.na-qwen { background: #615EFF; }
.na-features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.2rem;
}
.na-feature {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 1.5rem;
    transition: all 0.3s ease;
}
.na-feature:hover {
    border-color: rgba(59, 130, 246, 0.4);
    transform: translateY(-4px);
    box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
}
.na-feature-icon {
    width: 44px;
    height: 44px;
    background: var(--gradient-main);
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 1rem;
    font-size: 1.2rem;
}
.na-feature-title {
    font-size: 1.1rem;
    font-weight: 600;
    margin-bottom: 0.5rem;
    color: var(--text-primary);
}
.na-feature-desc {
    color: var(--text-secondary);
    font-size: 0.9rem;
    line-height: 1.6;
}
@media (max-width: 768px) {
    .na-home { padding: 1rem; }
    .na-title { font-size: 1.8rem; }
    .na-buttons { flex-direction: column; align-items: center; }
    .na-btn { width: 100%; max-width: 250px; justify-content: center; }
}
</style>

<div class="na-home">

<div class="na-hero">
<div class="na-badge">
<span class="na-badge-dot"></span>
<span>v3.0 全新发布 · 开源免费</span>
</div>

<h1 class="na-title">统一管理您的 AI 模型接口</h1>

<p class="na-desc">
企业级 API 分发与管理平台，<strong>一次接入</strong>即可调用 OpenAI、Claude、Gemini 等 <strong>50+ 主流模型</strong>，完全兼容 OpenAI 接口格式
</p>

<div class="na-buttons">
<a href="/register" class="na-btn na-btn-primary">🚀 免费开始</a>
<a href="/doc" class="na-btn na-btn-secondary">📖 查看文档</a>
</div>
</div>

<div class="na-stats">
<div class="na-stat">
<div class="na-stat-value">50+</div>
<div class="na-stat-label">支持模型</div>
</div>
<div class="na-stat">
<div class="na-stat-value">99.9%</div>
<div class="na-stat-label">服务可用性</div>
</div>
<div class="na-stat">
<div class="na-stat-value">&lt;50ms</div>
<div class="na-stat-label">平均延迟</div>
</div>
<div class="na-stat">
<div class="na-stat-value">10K+</div>
<div class="na-stat-label">活跃用户</div>
</div>
</div>

<div class="na-section">
<h2 class="na-section-title">支持主流 AI 模型</h2>
<p class="na-section-desc">统一接口格式，无缝切换不同模型</p>
<div class="na-models">
<div class="na-model"><span class="na-model-icon na-openai">AI</span> GPT-4o</div>
<div class="na-model"><span class="na-model-icon na-openai">AI</span> GPT-4 Turbo</div>
<div class="na-model"><span class="na-model-icon na-claude">C</span> Claude 3.5</div>
<div class="na-model"><span class="na-model-icon na-claude">C</span> Claude 3 Opus</div>
<div class="na-model"><span class="na-model-icon na-gemini">G</span> Gemini 1.5 Pro</div>
<div class="na-model"><span class="na-model-icon na-llama">L</span> Llama 3.1</div>
<div class="na-model"><span class="na-model-icon na-mistral">M</span> Mistral Large</div>
<div class="na-model"><span class="na-model-icon na-qwen">Q</span> Qwen2 72B</div>
</div>
</div>

<div class="na-section">
<h2 class="na-section-title">强大的功能特性</h2>
<p class="na-section-desc">为开发者和企业打造的一站式 AI 接口管理平台</p>
<div class="na-features">
<div class="na-feature">
<div class="na-feature-icon">🔄</div>
<h3 class="na-feature-title">多模型聚合</h3>
<p class="na-feature-desc">一个 API 调用所有主流 AI 模型，OpenAI 兼容格式，无需修改现有代码即可接入。</p>
</div>
<div class="na-feature">
<div class="na-feature-icon">💰</div>
<h3 class="na-feature-title">精细化计费</h3>
<p class="na-feature-desc">按 Token 计费，支持预付费和后付费模式，实时额度监控，精准控制成本。</p>
</div>
<div class="na-feature">
<div class="na-feature-icon">🔑</div>
<h3 class="na-feature-title">密钥轮询</h3>
<p class="na-feature-desc">支持多密钥负载均衡，自动故障转移，智能路由选择最优节点。</p>
</div>
<div class="na-feature">
<div class="na-feature-icon">📊</div>
<h3 class="na-feature-title">数据分析</h3>
<p class="na-feature-desc">详细的调用日志和数据可视化看板，帮助您深入了解 API 使用情况。</p>
</div>
<div class="na-feature">
<div class="na-feature-icon">⚡</div>
<h3 class="na-feature-title">流式响应</h3>
<p class="na-feature-desc">完整支持 SSE 流式传输，实时返回生成内容，提升用户体验。</p>
</div>
<div class="na-feature">
<div class="na-feature-icon">🛡️</div>
<h3 class="na-feature-title">安全可靠</h3>
<p class="na-feature-desc">企业级权限管控，完整审计日志，数据加密传输，保障您的数据安全。</p>
</div>
</div>
</div>

</div>
