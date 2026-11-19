# 贡献指南 / Contributing

感谢参与。建议提交前先检索现有 Issues 和 Pull Requests，避免重复工作。

1. **提出问题**：描述预期、实际结果、最小复现步骤、运行环境和可公开的日志；日志和截图需脱敏。
2. **讨论设计**：较大功能、破坏性变更或架构调整先开 Issue，明确范围和验收标准。
3. **创建分支**：按目标仓库的分支规范创建短期工作分支。**各项目分支策略以项目自己的文档为准**。
4. **提交 PR**：说明目的、变更、相关 Issue、实际执行的测试、兼容性及回滚方式；必要时附界面证据。
5. **维护者审核**：PR 至少经过适当测试与人工审查。CI 通过不等于自动批准，更不意味着所有依赖升级都应合并。

请勿上传访问令牌、密钥、个人数据、未授权采集数据或未脱敏的生产日志。安全漏洞请遵循 `SECURITY.md`，不要在公开 Issue 中披露利用细节。

## Commits

推荐使用 Conventional Commits：`feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `chore:`。项目可单独约定范围或语言。

## English summary

Search existing issues first. Include reproducible details without secrets or personal data. Discuss significant features before implementation. Follow repository-specific branch and testing instructions. Describe changes, verification, risks, and rollback in PRs. Maintainer review is required; passing CI alone does not authorize merging.
