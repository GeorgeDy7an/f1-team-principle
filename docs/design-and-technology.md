# Design and Technology / 设计思路与技术

## Design goal / 设计目标

The game compresses motorsport management into a fast decision-making experience. Players do not drive cars or wait for a lap-by-lap simulation. Instead, they make choices about drivers, development and resources, then see the consequences in race results and season reports.

游戏将复杂赛事经营压缩成可以快速推进的决策体验。玩家不需要操作赛车或等待逐圈模拟，而是在车手、研发和资源上作出选择，再从比赛结果与赛季报告中理解影响。

## The season loop / 赛季节奏

The full game begins each season with driver and development planning. Players can simulate races one at a time or advance to the next decision. A small number of race events and a mid-season review interrupt the simulation; a final-race decision can appear when an important championship or team-position outcome remains undecided. Season results and development feedback lead into the next year.

完整作品每年以车手与研发计划开始。玩家可以逐站模拟，也可以直接推进到下一个决策点。赛季中有少量比赛事件和一次阶段调整；当末站仍有重要冠军或车队名次悬念时，还可能出现额外决策。赛季结束后展示成绩与成长，再进入下一年。

This structure separates quickly reviewing results from moments that need thought. Feedback revealed that reducing the number of top-level decision points is not enough: the number and clarity of screens inside each point also matter.

这一结构将快速浏览结果与需要思考的时刻分开。实际反馈也表明，仅减少顶层节点数量并不够：每个节点内部的页面数量与操作清晰度同样影响节奏。

## Systems / 核心系统

| System / 系统 | Design / 设计 |
|---|---|
| Race simulation / 比赛模拟 | Car and driver ability, player decisions and controlled randomness produce final results. Exceptional races receive explanatory labels; weather, safety cars and incidents are not simulated lap by lap. / 赛车与车手能力、玩家决策和受控随机性共同生成最终结果。异常赛事使用解释标签，不逐圈模拟天气、安全车或事故。 |
| Decisions and resources / 决策与资源 | Pre-season, mid-season and event choices influence preparation, development or resource pressure. One-race effects and longer-term effects are tracked separately. / 季前、季中及事件选择影响准备、培养或资源压力，单站效果与长期效果分别记录。 |
| Driver and team world / 车手与车队世界 | Contracts, recruitment, driver development and car performance evolve across seasons, giving management choices lasting consequences. / 合同、新人、车手成长及赛车表现跨赛季变化，让经营决定产生延续性。 |
| Personality and feedback / 人格与反馈 | Changes in ability, personality labels and narrative reactions make development visible while some underlying information remains hidden. / 通过能力变化、人格标签和叙事反应呈现成长；部分底层信息保持隐藏。 |
| Season and career review / 赛季与生涯总结 | Results are considered alongside progress relative to the team's starting point, giving rebuilding and championship challenges different goals. / 除成绩外，也关注车队相对自身起点的进步，让弱队重建与强队争冠有不同目标。 |

## Technical trade-offs / 技术取舍

The browser-based game uses HTML, CSS and JavaScript rather than a real-time racing engine. Result-level simulation combines ability, choices and randomness to support both understandable patterns and occasional upsets. Mobile design iterations introduced pagination, consistent progression controls and separate detail views for dense information.

游戏在浏览器中使用 HTML、CSS 和 JavaScript，而不是实时赛车引擎。结果级模拟结合能力、选择与随机性，既保留可理解的实力规律，也允许偶发冷门。移动端迭代引入分页、一致的推进操作，并把复杂信息放入独立详情视图。

The public demo is a separately built illustration of **decision → simulation → feedback**. Its fictional data and calculations are not the full game's internal implementation.

公开演示是为解释**决策 → 模拟 → 反馈**而单独制作的示例；其虚构数据与计算方式并不代表完整作品的内部实现。

## Ongoing challenges / 仍需改进

Dense management information competes with limited mobile screen space. Accessibility on small displays, repeated events, clarity of decision feedback and long-term balance all need continued attention. Statistical simulations help identify patterns but cannot replace testing with players and real devices.

复杂经营信息与手机屏幕空间之间存在取舍。小屏可访问性、事件重复、决策反馈的清晰度和长期平衡仍需持续改进。批量模拟有助于发现统计规律，但不能代替真实设备与玩家测试。
