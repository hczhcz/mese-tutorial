MESE 讨论新编
===

1 基本概念
---

### 1.1 概述

MESE 全称 Management and Economics Simulation Exercise，最初是哈佛大学制作、用于教学的商业模拟软件。在上世纪末本世纪初，JA 组织广泛地使用这套软件来进行高中、大学经济学课程（JA Economics）教学。

本文讨论的 MESE 包括最初哈佛与 JA 的 MESE，也包括 JA Titan、IMese 和 MESE-Next，这三者都是支持网上对战的 MESE 变种。在默认情况下，本文讨论 2002 年之前的 MESE，不同之处会专门指出。

在 MESE 中，若干玩家分别组成虚拟的公司，在同一个市场中，生产并销售一种产品。MESE 是一种按期进行的模拟比赛，或者说是“回合制”的。每一期中，玩家要阅读自己公司以及整个行业的报表，并进行决策。比赛最终的目标称为 MPI（MESE Performance Index），在指定的期数后，获得最高 MPI 的玩家获胜。

### 1.2 五项决策

每一期中，玩家要进行五项决策，分别为价格（Price）、生产量（Prod）、营销投资（Mk）、生产投资（CI）、研发投资（RD）。

价格，即虚拟公司产品的售价。更高的价格意味着每卖出一个产品可以获得更多收入，但相应地，订单总数会减少。而较低的价格正好相反，意味着订单数量的增加，薄利多销。选定合适的价格，为自己生产的产品打开销路，并获得尽可能高的利润，是十分重要的。

生产量（产量），即公司生产的产品数。每个虚拟公司都有一定的生产能力（产能），高产量意味着公司有更多的可出售的产品，可以配合较低的价格来获得更多销售额和利润。但高产量的代价是，产品的生产成本会显著增加，减少利润。综合以上的效应，玩家需要通过计算和分析来确定一个合理的产量。MESE 中有一个“平衡开工率”，默认为 80%，即产量为产能的八成。低于此的产量很少出现，因为过低的开工率也意味着成本的急剧上升。一个例外是，如果公司遇到滞销或产能过剩，出现大量存货，玩家可以通过 0 开工快速清空存货。

Mk（营销投资的缩写，后文不再重复）是公司进行市场竞争的直接手段，更多的 Mk 意味着更多的订单。Mk 是单期起效的，本期的 Mk 只在本期发挥作用，在下期不再能够带来任何订单。Mk 的竞争性较强，高投入会意味着更高的收获，但如果整个市场都投入了大量的 Mk，那 Mk 能带来的订单数就会非常有限。因此，要避免在赢利预期不利的情况下投入过多 Mk，以免投资打水漂。另外，Mk 的效果与价格有关，低价高 Mk 效果最佳，但也意味着平均每个产品的利润极少。

CI 即通过投资获得更多的产能。MESE 有“折旧”的概念，CI 虽然消耗了资金，但它并不会立刻成为公司的成本，而是每一期按一定比例逐渐折算进成本。MESE 假设生产设备损坏的速度和折旧相同。产能的扩大意味着公司可以生产、销售更多产品，而且生产成本也会有所降低。但过度冗余的产能会使公司库存过多，也会增加折旧成本，而且多余的产能不能直接变现，只能逐渐通过折旧消耗。

RD 在原理上类似于 Mk，但它的作用效果来自每期平均值，而且与价格无关。RD 体现的是公司的技术积累，只有长期大量投入才能起到最好的效果。通常来说，RD 的决策决定了公司的战略，高 RD 代表了高投入、高利润率、前期落后后期追赶，而低 RD 正好相反。基于 MESE 的设定，RD 投资通常都在前几期，后期不再有任何投入。因为每一期 RD 的效果等价，前期投资 RD 意味着这笔投资能在更多期数产生作用，而最后一期的 RD 只在当期生效，几乎无法收回成本。

### 1.3 MPI

MPI 由六项指标组成。首先是留存利润，留存利润即每期利润之和，利润由销售额减去各项成本组成，但不包括 CI（CI 通过折旧，分摊计入各期成本），存货的生产成本也不计入当期成本。通常情况下留存利润是 MPI 的决定性因素，获得显著多余其他玩家的利润即可在 MESE 中取得第一，但在竞争激烈的情况下，其它 MPI 指标会起到重要作用。

然后是五项较小的指标。第一、二项是与历史积累有关的指标，第一项是历史累积的 Mk 和 RD 投入之和，第二项是总产能。这两项指标由玩家的决策框架决定，一般不需要额外考虑。第三项是开工率，越接近平衡开工率指标越高，这意味着最后一期我们通常不会 0 开工。第四、五项是与最后一期的表现直接有关的指标，第四项是销售量，即当期卖出了多少产品。第五项是增长率，将本期与上期销量相除而得。在利润影响不大的情况下，最后一期可以适当降低价格、增加销量，来提高 MPI。

2 报表
---

### 2.1 报表结构

MESE，Titan，IMese，和 MESE-Next，分别有不同的报表系统，尽管结构有一定区别，但涵盖的内容大同小异。报表中有公司和行业两部分，公司报表显示玩家公司的各种数据，而行业报表会显示所有玩家数据之和或者平均值（IMese 和 MESE-Next），以及每个玩家的一小部分数据。公司报表中的数据会更完整一些，而行业报表会隐去一些各个公司的“商业机密”，需要玩家自己来分析。MESE 的公司、行业报表可以分别打印，也可以以上下结构排列在一张纸内。MESE-Next 比较特殊，公司和行业报表是列在同一个界面内的，分别用 You 和 Average 标出。

以 MESE 的报表为例，公司报表长这样：

    Income Statement            % Sales  Operations Reports
    ----------------            -------  ------------------
    Sales              $  15750    100%  Decisions: Price      $    30
    COGS               $  -9634     61%             Production     525 units
                      --------- -------             Marketing  $  1400
    Gross Margin       $   6116     39%             Investment $  1400
    Marketing          $  -1400      9%             R & D      $   525
    Depreciation       $  -1400      9%
    R & D              $   -525      3%
    Layoff Charge      $      0      0%  Production Report:
    Inventory Charge   $      0      0%  Production                525 units
    Interest           $   -199      1%  Factory Capacity          700 units
                      --------- -------  Capacity Utilization       75 %
    Profit before Tax  $   2592     16%  Production Cost/Unit  $ 18.35
    Tax                $   -648      4%  Inventory                   0 units
                      --------- -------  Employees                 105 workers
    Net Profit         $   1944     12%

    Balance Sheet               % Total  Marketing Report:
    -------------               -------  Orders Received           525 units
    Cash               $  13503     33%  Sales Made                525 units
    Inventory          $      0      0%  Unfilled Orders             0 units
    Capital Investment $  28000     67%  Price/Unit Sold       $ 30.00
                      --------- -------  Total Cost/Unit Sold  $ 25.06
    Total Assets       $  41503    100%  Margin/Unit Sold      $  4.94

    Loans              $   7254     17%  Investment Report:
    Retained Earnings  $   3799      9%  Factory Size     $  28000     700 units
    Capital            $  30450     73%  Net Investment   $      0       0 units
                      --------- -------                   --------- ------
    Liabilities+Equity $  41503    100%  Size Next Period $  28000     700 units

行业报表长这样：

    Units                       Change    Dollars                         Change
    -----                       ------    -------                         ------
    Total Orders        3150        0%    Industry Sales         $ 94500      0%
    Total Produced      3150        0%    Average Price          $ 30.00      0%
    Total Sold          3150        0%    Total Production       $ 57802      0%
    Total Capacity      4200        0%    Avg Pdtn Cost          $ 18.35      0%
    Inventory              0        0%    Avg Total Cost         $ 25.06      0%

    Productivity                Change    Dollars                         Change
    ------------                ------    -------                         ------
    Employment           630        0%    Prime Rate                 10%      0%
    Sales/Employee  $    150        0%    Loan Limit             $ 50000      0%
    Units/Employee      5.00        0%    Tax Rate                   25%      0%
    Cap. Investment $ 168000        0%    Tax Paid in Period     $  3888      5%
    Capacity Util.       75%        0%    Tax Paid to Date       $  7596    105%

           PLAYER 1 PLAYER 2 PLAYER 3 PLAYER 4 PLAYER 5 PLAYER 6
           -------- -------- -------- -------- -------- --------
    Sales   $ 15750  $ 15750  $ 15750  $ 15750  $ 15750  $ 15750
    Profit  $  1944  $  1944  $  1944  $  1944  $  1944  $  1944
    Price   $    30  $    30  $    30  $    30  $    30  $    30
    RetErn  $  3799  $  3799  $  3799  $  3799  $  3799  $  3799
    Un Shr      17%      17%      17%      17%      17%      17%
    MPI         101      101      101      101      101      101

下面，我们分块来看。

### 2.2 生产与销售

公司生产与产能状况：

    Production Report:
    Production                525 units
    Factory Capacity          700 units
    Capacity Utilization       75 %
    Production Cost/Unit  $ 18.35
    Inventory                   0 units
    Employees                 105 workers

    Investment Report:
    Factory Size     $  28000     700 units
    Net Investment   $      0       0 units
                     --------- ------
    Size Next Period $  28000     700 units

Production 和 Factory Capacity 分别是产量和产能，将它们相除即可得到开工率。Production Cost/Unit 即每个产品平均的生产成本，在 MESE-Next 中，还有一项边际成本，指的是多生产一件产品会增加的额外生产成本。当开工率为 80% 时，平均生产成本等于边际成本，这是最省钱的生产方式。但在早期，公司的产能往往不足，往往需要更高的开工率来弥补。接下来是库存，有库存意味着之前生产的产品没有售罄。最后一项是公司的雇员数，它与开工率有关。

Net Investment 表示 CI 减去折旧的值，也就是新增的产能。这张报表中 CI 恰好与折旧相等，所以新的一期里，产能并没有发生变化。

公司销售状况：

    Marketing Report:
    Orders Received           525 units
    Sales Made                525 units
    Unfilled Orders             0 units
    Price/Unit Sold       $ 30.00
    Total Cost/Unit Sold  $ 25.06
    Margin/Unit Sold      $  4.94

公司的客户会向公司订货，即 Orders，如果公司的产量和之前的库存之和足够多，就能满足全部订单，并留下更多库存（就是上面的 Inventory 项）。但如果没有足够的产品可供出售，就会引发 Unfilled Orders，俗称 UFO。库存和 UFO 是供需不平衡的两面，太多库存意味着产能过剩或者销路不畅，而 UFO 正好相反。但需要注意，脱销并不是好事，而是意味着赚少了：公司的产品本可以卖得更贵，或者投入更少 Mk 和 RD。之后是价格、平均花费和利润，价格减去花费得到利润，这很好理解。

行业数据与公司的数据对应，不再赘述：

    Units                       Change
    -----                       ------
    Total Orders        3150        0%
    Total Produced      3150        0%
    Total Sold          3150        0%
    Total Capacity      4200        0%
    Inventory              0        0%

    Productivity                Change
    ------------                ------
    Employment           630        0%
    Sales/Employee  $    150        0%
    Units/Employee      5.00        0%
    Cap. Investment $ 168000        0%
    Capacity Util.       75%        0%

MESE-Next 中，这些数据显示在 Production，Units 和 Balance（一部分）区域中：

    Production           You   Average
    Prod rate            0.8
    Unit prod cost        18        18
    Marginal cost         18
    Total prod cost     7560      7560

    Units                You   Average
    Orders               420       420
    Units sold           420       420
    Inventory              0         0
    Unfilled               0         0

    Balance              You   Average
    Deprecation         1050
    Capital            21000     21000
    Size                 525       525

### 2.3 资金与利润

### 2.4 其它信息

3 决策流程
---

4 宏观与战略
---

5 具体战术
---

6 比赛与团队
---

7 高级话题
---
