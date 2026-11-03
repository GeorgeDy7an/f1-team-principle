# Development and Validation / 开发历程与验证

## From concept to prototype / 从构想到可玩原型

1. **Define the core experience.** Focus on team management, fast seasons and a small number of key choices, without lap-by-lap simulation or direct driving.  
   **确定核心体验。** 聚焦车队经营、快速赛季和少量关键决策，不做逐圈模拟或直接驾驶。
2. **Prototype race results.** Combine car and driver ability with random variation, retirements and occasional upsets. Early versions used batch simulation to inspect result distributions.  
   **建立比赛原型。** 结合赛车与车手能力、随机波动、退赛和少量冷门；早期版本通过批量模拟观察成绩分布。
3. **Connect seasons.** Add car development, driver growth, contracts and recruitment so that choices can carry forward.  
   **连接赛季。** 加入赛车研发、车手成长、合同和新人市场，让选择的影响延续到未来。
4. **Build career feedback.** Add personality reactions, season reports and a ten-year review to reflect different achievements, from titles to rebuilding.  
   **建立生涯反馈。** 加入人格反应、赛季报告和十年总结，呈现争冠与重建等不同成果。
5. **Iterate on mobile usability.** Player feedback exposed long screens, obscured buttons and unclear recruitment flows. Pagination, layout and step-by-step interactions were revised.  
   **根据反馈改善手机体验。** 玩家指出页面过长、按钮被遮挡、招募逻辑难理解；因此反复调整分页、布局与操作步骤。
6. **Create an offline bilingual edition.** Remove platform dependencies, add Chinese/English selection and check offline play, saves and several mobile viewport sizes.  
   **制作离线双语版。** 移除平台依赖，加入中英文切换，并检查离线玩法、存档和多种手机视口。

## Validation / 验证方式

- Fixed-seed batch simulations were used to inspect points, win rates, retirements and upsets. Historical figures belong to the version and parameters tested at the time; they should not be presented as current balance results.  
  使用固定随机种子的批量模拟观察积分、胜率、退赛和冷门；历史数字只对应当时的版本与参数，不能当作当前版本的平衡结果。
- Desktop-browser mobile viewports were used to test key screens, selections and button access. Offline checks blocked network requests while testing the game and its local resources.  
  在桌面浏览器的手机视口中测试主要页面、选择与按钮可访问性；离线检查通过阻断网络请求验证游戏及本地资源。
- Scripts checked season progression, ten-year career boundaries, roster constraints and save recovery. These checks cover selected scenarios; passing them does not prove compatibility with every device or random branch.  
  脚本检查了赛季推进、十年生涯边界、阵容约束和存档恢复。这些测试覆盖的是选定场景，不能证明所有设备与随机分支都已验证。

## Roles and approach / 分工与方法

GEORGE led the gameplay direction, user-experience requirements and iteration decisions. AI assisted with code implementation, debugging and testing; feedback from actual interface use informed subsequent changes.

GEORGE 主导玩法方向、用户体验要求和迭代决策；AI 辅助代码实现、调试与测试，并依据实际界面使用反馈持续调整。

This portfolio focuses on design decisions, problem finding and iteration. The public example does not contain the complete game code.

本作品集着重展示设计取舍、问题定位与迭代方法；公开示例不包含完整游戏代码。
