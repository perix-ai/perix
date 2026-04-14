# Perix

Perix 云端核心系统主仓。

## 仓库定位
承载云端核心能力：
- Gateway / API Server / Actor Runtime / Scheduler
- Agent Runtime / Orchestrator / Tool Engine / Skills Runtime
- Memory / User Model / Push Engine / Evolution / LLM Gateway
- Auth / Governance
- DB Migrations / Deploy / Docs

## 目录结构
```text
apps/
  gateway/
  api-server/
  actor-runtime/
  scheduler/
modules/
  orchestrator/
  agent-runtime/
  tool-engine/
  skills-runtime/
  memory/
  user-model/
  push-engine/
  evolution/
  llm-gateway/
  auth/
  governance/
schemas/
  openapi/
  protobuf/
db/
  migrations/
  seeds/
deploy/
  docker/
  k8s/
  helm/
docs/
```

## 建议
- 单仓承载云端核心，避免早期过度拆分
- 服务可以独立部署，但代码先保持同仓演进
- 稳定后再按真实团队边界拆仓
