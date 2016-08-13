MESE 讨论新编
===

1 基本概念
---

### 1.1 概述

MESE 全称 Management and Economics Simulation Exercise，最初是哈佛大学制作、用于教学的商业模拟软件。在上世纪末本世纪初，JA 组织广泛地使用这套软件来进行高中、大学经济学课程（JA Economics）教学。

在 MESE 商业模拟赛事中，若干玩家分别组成虚拟的公司，生产并销售一种产品（MESE 默认设定的产品是“记忆笔”，这是一种存在于未来的高科技文具），并在同一个市场里竞争。玩家需要阅读报表，制定公司的决策，并尽力使公司取得较好的表现。

本文讨论的 MESE 包括最初哈佛与 JA 的 MESE，也包括 JA Titan、IMese 和 MESE-Next，这三者都是支持网上对战的 MESE 变种。在默认情况下，本文讨论 2002 年之前的 MESE，上述的变种和 MESE 在许多方面是相同或相似的，不同之处会专门指出。

### 1.2 赛制

MESE 是一种按期进行的模拟比赛，或者说是“回合制”的，一期代表一个季度。每一期中，玩家要阅读自己公司以及整个行业的报表，然后提交决策。比赛最终的目标称为 MPI（MESE Performance Index），在比赛进行到指定的期数后，获得最高 MPI 的玩家获胜。

有几种赛制常见于 MESE 及其变种。首先是定时赛，这种类型的赛事会规定一个每期时限，玩家需要在若干分钟的时限内提交决策。如果玩家决策超时，会面临强制使用默认决策或取消比赛资格等处罚。第二种是长期赛，与定时赛规定时间不同，这类赛事每期会有若干天可以用于决策，期间可以进行大量的分析和计算工作。第三种是即时赛，所有玩家提交决策后即进入下一期，常见于网上局。

有的赛事中，玩家会收到关于经济走势的提示，一般称为“宏观”，可用于判断未来市场走向。另一些赛事会使用固定的市场模型，例如 Titan 中的剧本，和网上局使用的 343、262 设定等。

MESE 赛事的总期数通常在六到八之间，有事先规定期数的，也有现场随机决定的。Titan 赛事的期数更多一些，可以到九到十二。而国内的 MESE 网上局（IMese 和 MESE-Next）一般进行七期。

### 1.3 五项决策

每一期中，玩家要提交五项决策，分别为价格（Price）、生产量（Prod）、营销投资（Mk）、生产投资（CI）、研发投资（RD）。

价格，即虚拟公司产品的售价。更高的价格意味着每卖出一个产品可以获得更多收入，但相应地，订单总数会减少。而较低的价格正好相反，意味着订单数量的增加，薄利多销。选定合适的价格，为自己生产的产品打开销路，并获得尽可能高的利润，是十分重要的。

生产量（产量），即公司生产的产品数。每个虚拟公司都有一定的生产能力（产能），高产量意味着公司有更多的可出售的产品，可以配合较低的价格来获得更多销售额和利润。但高产量的代价是，产品的生产成本会显著增加，减少利润。综合以上的效应，玩家需要通过计算和分析来确定一个合理的产量。MESE 中有一个“平衡开工率”，默认为 80%，即产量为产能的八成。低于此的产量很少出现，因为过低的开工率也意味着成本的急剧上升。一个例外是，如果公司遇到滞销或产能过剩，出现大量存货，玩家可以通过 0 开工快速清空存货。

Mk（营销投资的缩写，后文不再重复）是公司进行市场竞争的直接手段，更多的 Mk 意味着更多的订单。Mk 是单期起效的，本期的 Mk 只在本期发挥作用，在下期不再能够带来任何订单。Mk 的竞争性较强，高投入会意味着更高的收获，但如果整个市场都投入了大量的 Mk，那 Mk 能带来的订单数就会非常有限。因此，要避免在赢利预期不利的情况下投入过多 Mk，以免投资打水漂。另外，Mk 的效果与价格有关，低价高 Mk 效果最佳，但也意味着平均每个产品的利润极少。Titan 的 Mk 有细节选项，作用原理暂时不明，根据经验，一般选择可选项目中门槛最高的。

CI 即通过投资获得更多的产能。MESE 有“折旧”的概念，CI 虽然消耗了资金，但它并不会立刻成为公司的成本，而是每一期按一定比例逐渐折算进成本。MESE 假设生产设备损坏的速度和折旧相同。产能的扩大意味着公司可以生产、销售更多产品，而且生产成本也会有所降低。但过度冗余的产能会使公司存货过多，也会增加折旧成本，而且多余的产能不能直接变现，只能逐渐通过折旧消耗。

RD 在原理上类似于 Mk，但它的作用效果来自每期平均值，而且与价格无关。RD 体现的是公司的技术积累，只有长期大量投入才能起到最好的效果。通常来说，RD 的决策决定了公司的战略，高 RD 代表了高投入、高利润率、前期落后后期追赶，而低 RD 正好相反。基于 MESE 的设定，RD 投资通常都在前几期，后期不再有任何投入。因为每一期 RD 的效果等价，前期投资 RD 意味着这笔投资能在更多期数产生作用，而最后一期的 RD 只在当期生效，几乎无法收回成本。Titan 的 RD 也有细节选项，较少玩家研发出来的功能可以带来少许优势。可以观察新闻栏，选择其它公司还未研发出来的功能进行尝试。

Titan 还有第六项决策是慈善投入，这一项是教育用途的，唯一的效果是增加少量订单，因此投满即可。

### 1.4 MPI

MPI 由六项指标组成。首先是留存利润，留存利润即每期利润之和，利润由销售额减去各项成本组成，但不包括 CI（CI 通过折旧，分摊计入各期成本），存货的生产成本也不计入当期成本。通常情况下留存利润是 MPI 的决定性因素，获得显著多余其他玩家的利润即可在 MESE 中取得第一，但在竞争激烈的情况下，其它 MPI 指标会起到重要作用。

然后是五项较小的指标。第一、二项是与历史积累有关的指标，第一项是历史累计的 Mk 和 RD 投入之和，第二项是总产能。这两项指标由玩家的决策框架决定，一般不需要额外考虑。第三项是开工率，越接近平衡开工率指标越高，这意味着最后一期我们通常不会 0 开工。第四、五项是与最后一期的表现直接有关的指标，第四项是销量，即当期卖出了多少产品。第五项是增长率，将本期与上期销量相除而得，但有一定上限。在利润影响不大的情况下，最后一期可以适当降低价格、增加销量，来提高 MPI。

2 报表
---

### 2.1 报表结构

MESE，Titan，IMese，和 MESE-Next，分别有不同的报表系统，尽管结构有一定区别，但涵盖的内容大同小异。报表中有公司和行业两部分，公司报表显示玩家公司的各种数据，而行业报表会显示所有玩家数据之和或者平均值（IMese 和 MESE-Next），以及每个玩家的一小部分数据。公司报表中的数据会更完整一些，而行业报表会隐去一些各个公司的“商业机密”，需要玩家自己来分析。MESE 的公司、行业报表可以分别打印，也可以以上下结构排列在一张纸内。

Titan 的报表结构和 MESE 很接近，IMese 的也大同小异，只是需要注意行业报表默认显示的是平均值而不是总和。MESE-Next 比较特殊，公司和行业报表是列在同一个界面内的，分别用 You 和 Average 标出。而且，MESE-Next 的报表数据分为 Early 和 Result 两类，分别表示在期初（生产、投资阶段）和期末（销售阶段）产生的数据。对于不同之处，下文会单独指出。

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

MESE 的完整报表还包括现金流表和提示信息，但主要是出于教学目的，此处略过。下面，我们分块来看。

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

Production 和 Factory Capacity 分别是产量和产能，将它们相除即可得到开工率。Production Cost/Unit 即每个产品的生产成本，在 MESE-Next 中，还有一项边际成本，指的是多生产一件产品会增加的额外生产成本。当开工率为 80% 时，单位生产成本等于边际成本，这是最省钱的生产方式，例如上面的报表中，如果生产 700 的 80%，即 560 个，单位生产成本可以降到 18。但在早期，公司的产能不足，往往需要更高的开工率来弥补。接下来是存货，有存货意味着之前生产的产品没有售罄。最后一项是公司的雇员数，它与开工率有关。

通过 Investment Report 可以看出，一个单位产能的价值等于 28000 除以 700，得 40。Net Investment 表示 CI 减去折旧的值，也就是新增的产能。这张报表中，CI 决策恰好与折旧相等，都是 1400，所以新的一期里，产能并没有发生变化。

公司销售状况：

    Marketing Report:
    Orders Received           525 units
    Sales Made                525 units
    Unfilled Orders             0 units
    Price/Unit Sold       $ 30.00
    Total Cost/Unit Sold  $ 25.06
    Margin/Unit Sold      $  4.94

公司的客户会向公司订货，即 Orders，如果公司的产量和之前的存货之和足够多，就能满足全部订单，并留下新的存货（就是上面的 Inventory 项）。但如果没有足够的产品可供出售，就会引发 Unfilled Orders，俗称 UFO。存货和 UFO 是供需不平衡的两面，太多存货意味着产能过剩或者销路不畅，而 UFO 正好相反。但需要注意，脱销并不是好事，而是意味着赚少了：公司的产品本可以卖得更贵，或者投入更少 Mk 和 RD。之后是价格、每个产品的平均花费和利润，价格减去花费得到利润，这很好理解。

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

    Early Report

    Production           You   Average
    Prod rate            0.8
    Unit prod cost        18        18
    Marginal cost         18
    Total prod cost     7560      7560

    Balance              You   Average
    Deprecation         1050
    Capital            21000     21000
    Size                 525       525

    Result Report

    Units                You   Average
    Orders               420       420
    Units sold           420       420
    Inventory              0         0
    Unfilled               0         0

### 2.3 资金与利润

收支表，这张表本质上是从 Sales 开始向下做加减法，最终算出利润：

    Income Statement            % Sales
    ----------------            -------
    Sales              $  15750    100%
    COGS               $  -9634     61%
                      --------- -------
    Gross Margin       $   6116     39%
    Marketing          $  -1400      9%
    Depreciation       $  -1400      9%
    R & D              $   -525      3%
    Layoff Charge      $      0      0%
    Inventory Charge   $      0      0%
    Interest           $   -199      1%
                      --------- -------
    Profit before Tax  $   2592     16%
    Tax                $   -648      4%
                      --------- -------
    Net Profit         $   1944     12%

首先是 Sales，即总销售额，销量和单价的乘积。COGS 是售出产品的生产成本，MESE 对 COGS 的计算采用加权平均的策略，假定存货和新生产的产品按相同的比率出货。假设现在有 500 个存货，产量 1000，销量 1200，那么存货和新品分别出货 400 和 800，100 原有存货和 200 的新品组成新一期的存货。Sales 和 COGS 相减得到毛利润。

之后是各项花费，可以看到 Mk 和 RD 直接计入了成本，而 CI 是应用到 Factory Size 里，然后按一定比例（每期 5%）的折旧计入的。Layoff Charge 是当雇员数减少时产生的裁员费。Inventory Charge 是存货费，取连续两期中存货量的较小值来计算，例如上期存 100，本期存 200，则按 100 个存货来计价。公司持有的现金和背负的贷款会产生利息。以上共同计算得到税前利润，扣除固定税率的税之后就得到公司的利润了。

资金平衡表：

    Balance Sheet               % Total
    -------------               -------
    Cash               $  13503     33%
    Inventory          $      0      0%
    Capital Investment $  28000     67%
                      --------- -------
    Total Assets       $  41503    100%

    Loans              $   7254     17%
    Retained Earnings  $   3799      9%
    Capital            $  30450     73%
                      --------- -------
    Liabilities+Equity $  41503    100%

上半块的三项依次为现金、存货生产成本和总 CI（即是 Factory Size）。每期中，存货生产成本中会去掉 COGS，并加上新加入存货的产品的生产成本。类似地，总 CI 会去掉折旧，并加上新投入的 CI。

下半块的三项依次是贷款、留存利润和初始资本（是一个固定值）。一个看上去巧合的现象是，上三项之和等于下三项之和，但这实际上是 MESE 资金流的本质所决定的：一个公司的收入不是以现金存在，就是以实物存在，再不然就是还了贷款，不会凭空出现也不会凭空消失。

行业数据：

    Dollars                         Change
    -------                         ------
    Industry Sales         $ 94500      0%
    Average Price          $ 30.00      0%
    Total Production       $ 57802      0%
    Avg Pdtn Cost          $ 18.35      0%
    Avg Total Cost         $ 25.06      0%

    Dollars                         Change
    -------                         ------
    Prime Rate                 10%      0%
    Loan Limit             $ 50000      0%
    Tax Rate                   25%      0%
    Tax Paid in Period     $  3888      5%
    Tax Paid to Date       $  7596    105%

这里除了和公司数据一样的部分，还多了三项设定：Prime Rate 是参考年利率，存款和贷款利率是据此产生的，MESE 中存款的利率为贷款的一半。需要注意，MESE 的一期是一个季度，也就是 1/4 年，利息应该据此计算。在 MESE-Next 中，存款和贷款的利率是分别列出的，且不需要额外的计算。Loan Limit 是贷款限额，提交决策前需要算出自己将使用的贷款额度，避免贷款超限。Tax Rate 是税率。

MESE-Next 中，这些数据显示在 Goods 和 Balance（一部分）区域中：

    Early Report

    Goods                You   Average
    Goods                420       420
    Cost of goods       7560
    Ideal sales income 12600

    Balance              You   Average
    Deprecation         1050
    Capital            21000     21000
    Size                 525       525
    Spending            9030
    Early loan          7280
    Interest            -364

    Result Report

    Goods                You   Average
    Cost of goods sold  7560      7560
    Cost of inventory      0

    Balance              You   Average
    Sales income       12600     12600
    Cost before tax    10444     10444
    Profit before tax   2156      2156
    Profit              1617      1617
    Loan                7280
    Cash               10647
    Retained earning    1617      1617

这里还多了 Goods 的概念，表示存货和新品总和。Ideal sales income 是 Goods 和价格的乘积，表示如果售罄，公司将获得多少销售额。如果这个数值明显不符合经验，意味着可能有大量的存货或者 UFO 产生。

另外，MESE-Next 的报表中，设定是单列在 Settings 区域的。

### 2.4 玩家栏

之前的例子中，MESE 的玩家栏长这样：

           PLAYER 1 PLAYER 2 PLAYER 3 PLAYER 4 PLAYER 5 PLAYER 6
           -------- -------- -------- -------- -------- --------
    Sales   $ 15750  $ 15750  $ 15750  $ 15750  $ 15750  $ 15750
    Profit  $  1944  $  1944  $  1944  $  1944  $  1944  $  1944
    Price   $    30  $    30  $    30  $    30  $    30  $    30
    RetErn  $  3799  $  3799  $  3799  $  3799  $  3799  $  3799
    Un Shr      17%      17%      17%      17%      17%      17%
    MPI         101      101      101      101      101      101

从上到下依次是各个玩家公司的销售额、利润、产品价格、留存利润、市场份额和 MPI。MESE-Next 的玩家栏大同小异，少了市场份额，多了销量，以及不含税的本期花费。玩家栏是观察其他玩家的唯一窗口（两人局除外），尽管只有很少的数据，但通过合理的分析，我们可以大致计算出其他玩家的大部分报表内容，甚至推测出他们的决策，这是团队 MESE 中经常使用的技巧，称为“跟踪”。

3 流程与公式
---

### 3.1 运行流程

MESE 是按期运行的。每期中，玩家会先收到报表，随后提交五项（Titan 六项）决策，在每期关闭之前，玩家可以修改自己的决策。“关闭”一期，即是进行一个季度的模拟。一次模拟中会进行的操作包括生产、变更产能、分配订单、出货、计算 MPI 等，最后生成新的报表。

下面描述的是 MESE 及变种的内部运行流程。Titan 的运行流程不详，但除了少数几个例外，推测与 MESE 相同。IMese 使用 MESE 作为运算引擎，因此与 MESE 相同，不单独列出。

MESE 的运行流程并不是玩家必须了解的内容，可在之后介绍决策流程时比对参考。

### 3.2 生产与产能

首先是开工率，直接将产量除以产能就可以了。注意，这里的 last.size 是报表里的 Size Next Period，而报表里的 Factory Size 是再上一期的数据：

    prod_rate =
        decisions.prod / last.size
    prod_over =
        prod_rate - 0.8

生产成本，其中 init.capital 指初始资本：

    prod_cost_factor_rate =
        69 （MESE 和 Titan，高于平衡开工率）
        138 （MESE 和 Titan，低于平衡开工率）
        63 （MESE-Next）
    prod_cost_unit =
        prod_cost_factor_rate * prod_over ^ 2
        + 15 * init.capital / last.capital
        + 3
    prod_cost_marginal =
        prod_cost_factor_rate * 2 * prod_rate * prod_over + prod_cost_unit
    prod_cost =
        prod_cost_unit * decisions.prod

折旧，以及应用 CI 之后新的产能，其中每个产能单位价值为 40：

    deprecation =
        0.05 * last.capital
    capital =
        last.capital + decisions.ci - deprecation
    size =
        capital / 40

雇员和裁员费。裁员费的计算在 MESE 中是个经典的 bug，不扣钱反而加钱，而在 MESE-Next 中则直接取消了：

    employees =
        init.employees / init.prod_rate * prod_rate
    layoff_charge =
        (last.employees - employees) * 10 （MESE 和 Titan，有裁员）
        0 （MESE 和 Titan，无裁员）
        0 （MESE-Next）

### 3.3 出货

可供出售的产品，包括存货和新品：

    goods =
        last.inventory + decisions.prod
    goods_cost =
        last.goods_cost_inventory + prod_cost
    goods_max_sales =
        decisions.price * goods

通过订单分配机制，取得订单数 orders（订单分配在后文讲解），将产品售出：

    sold =
        orders （货多于订单，有存货）
        goods （货少于订单，售罄）
    inventory =
        goods - sold
    unfilled =
        orders - sold

计算售出产品和存货的生产成本，它们是从存货和新品的总生产成本中按比例分摊的：

    goods_cost_sold =
        goods_cost * sold / goods
    goods_cost_inventory =
        goods_cost - goods_cost_sold

销售额，可以和 goods_max_sales 相比较：

    sales =
        decisions.price * sold

存货费，默认每件的存货费为 1，按本期和上期之间存货较少的来算：

    inventory_charge =
        last.inventory （MESE 和 MESE-Next，上期存货较少）
        inventory （MESE 和 MESE-Next，本期存货较少）
        不明 （Titan）

### 3.4 订单分配

MESE 的订单分配分成两个步骤，其一是计算 demand，即市场总订单，其二是计算 share，即每家公司分得的订单。需要注意，Titan 的订单分配方式目前不明，尽管很可能与 MESE 相近。

先从 demand 开始。在 MESE 中，Mk 是对竞争敏感的，当市场总 Mk 较大时，Mk 的效果相应降低。这是通过一个两段式函数实现的，其中 sum 表示所有玩家数据之和：

    sum_mk_compressed =
        (sum(decisions.mk) - 2 * sum(init.mk)) / 4
        + 2 * sum(init.mk) （平均 Mk 大于 2 * init.mk）
        sum(decisions.mk) （否则）

在 MESE 中，有两种不同的均价计算方式，分别是直接按价格决策平均，和按预期销量加权平均。下面的 player_count 指玩家数：

    average_price_given =
        sum(decisions.price) / player_count
    average_price_planned =
        sum(goods_max_sales) / sum(goods)

当然，average_price_planned 只是预计的均价。到订单分配、出货完成后，还要计算一个实际的均价：

    average_price =
        sum(sales) / sum(sold) （在每期的最后计算）

将预期加权均价和上期的加权均价再按比例混合，就得到了用于订单分配的均价。其中的比例正是价格的 demand 设定：

    demand_price =
        1 （默认值）
    average_price_mixed =
        demand_price * average_price_planned
        + (1 - demand_price) * last.average_price

记录历史上投入过的 Mk 和 RD 的总和（包括当期），以备之后使用：

    history_mk =
        last.history_mk + decisions.mk
    history_rd =
        last.history_rd + decisions.rd

Demand 由 Mk 和 RD 的影响因素共同构成。价格和 Mk 共同构成 Mk 因素，而不单独发挥作用。RD 因素采用历史上每期投入 RD 的平均值来确定：

    demand_mk =
        5.3 （MESE，默认值）
        5 （MESE-Next，默认值）
    demand_effect_mk =
        demand_mk
        * sqrt(sum_mk_compressed / sum(init.mk))
        / (average_price_mixed / init.price)
    demand_rd =
        1 （默认值）
    demand_effect_rd =
        demand_rd
        * (sum(history_rd) / now_period / sum(init.rd))

算出预期的市场总订单数，以备之后的“瓜分”：

    demand =
        62.5 （MESE，默认值）
        70 （MESE-Next，默认值）
    orders_demand =
        demand * (demand_effect_rd + demand_effect_mk)

接下来是各玩家公司的 share，即市场份额的计算。Share 由价格、Mk 和 RD 三个成分构成，其中 Mk 成分与价格仍然有关：

    share_effect_price =
        (average_price_mixed / decisions.price) ^ 3
    share_effect_mk =
        (decisions.mk / decisions.price) ^ 1.5
    share_effect_rd =
        history_rd

三个 share 成分加权得到总 share。其中的权重是 MESE 最重要的设定之一，它决定了一场比赛的整体风格。常见的权重组合有：

    share_price : share_mk : share_rd =
        0.3  : 0.4 : 0.3  （MESE-Next 及 IMese 默认值，343 设定）
        0.2  : 0.5 : 0.3
        0.25 : 0.5 : 0.25
        0.2  : 0.6 : 0.2  （262 设定）
        0.15 : 0.7 : 0.15 （MESE 默认值）

据此计算出 share。对于价格高于 40 的情况，share 还会被限制，因此 40 是 MESE 中高端与低端市场的价格分界线。最后，demand 和 share 共同产生订单数：

    share =
        share_price * share_effect_price / sum(share_effect_price)
        + share_mk * share_effect_mk / sum(share_effect_mk)
        + share_rd * share_effect_rd / sum(share_effect_rd)
    share_compressed =
        share * 40 / decisions.price （价格高于 40）
        share （否则）
    orders = orders_demand * share_compressed

Titan 的 share 比较特殊，在计算之后还要进行取整，因此有“点位”的概念。有经验的玩家会利用取整带来的额外订单数，创造更高的利润。Titan 有慈善这项决策，会使订单总数稍许增加。另外，Mk 和 RD 的细节选项也会影响获得的订单数，但效果微弱。

### 3.5 现金流

除了价格，其它四项决策都是要花钱的。根据 MESE 现金流的逻辑，折旧是不计入花费的：

    spending =
        prod_cost + decisions.ci - deprecation + decisions.mk + decisions.rd

根据花费和上一期的现金、贷款，计算得到期初贷款：

    balance_early =
        last.cash - last.loan - spending
    loan_early =
        - balance_early （balance_early 为负，需要贷款）
        0 （balance_early 非负，现金结余）

如果 loan_early 超过贷款限额，决策就会被拒绝。

在 MESE 中，如果贷款还清了就计算存款利息，否则不计算存款利息、只计算贷款利息。而在 MESE-Next 中，利息是根据 balance_early 直接计算的：

    interest =
        interest_rate / 8 * last.cash （MESE 和 Titan，期初现金结余）
        interest_rate / 4 * loan_early （MESE 和 Titan，期初有贷款）
        interest_rate_cash * balance_early （MESE-Next，期初现金结余）
        interest_rate_loan * balance_early （MESE-Next，期初有贷款）

上面的计算都发生在期初，接下来是利润以及各项期末的数据的计算。先从税前利润开始：

    cost_before_tax =
        goods_cost_sold
        + deprecation
        + decisions.mk + decisions.rd
        - interest + inventory_charge + layoff_charge
    profit_before_tax =
        sales - cost_before_tax

然后按固定比例扣税：

    tax_charge =
        tax_rate * profit_before_tax
    profit =
        profit_before_tax - tax_charge

期末 balance，可以根据现金流计算：

    balance =
        balance_early + loan_early
        + sales - deprecation
        + interest - inventory_charge - layoff_charge - tax_charge

也可以从利润出发，排除折算项目来计算，两种方式本质上是相同的。MESE-Next 实际使用这种计算方式：

    balance =
        last.cash - last.loan + loan_early
        + profit - decisions.ci + deprecation + goods_cost_sold - prod_cost

进一步得到期末贷款和现金：

    loan =
        loan_early （期末 balance 为正）
        loan_early - balance （否则）
    cash =
        balance （期末 balance 为正）
        0 （否则）

留存利润为每期利润之和：

    retern =
        last.retern + profit

### 3.6 MPI

留存利润，按每期平均值计算，并且没有上限：

    mpi_a =
        50 * retern / now_period / init.retern

历史投入的 Mk 和 RD 占所有玩家比例：

    mpi_b =
        10 * (history_rd + history_mk)
        / (sum(history_rd) + sum(history_mk)) * player_count

产能占所有玩家比例：

    mpi_c =
        10 * size / sum(size) * player_count

开工率，每多于或少于平衡开工率十个百分点，MPI 减 1。考虑到取整，75% 到 85% 的开工率对应满 MPI：

    mpi_d =
        10 * (1 - |prod_over|)

销量占所言玩家比例：

    mpi_e =
        10 * sold / sum(sold) * player_count

增长率，上限为 20。一些玩家会在最后一期大幅减价，来获得 MPI：

    mpi_f =
        10 * sold / last.sold
        / sum(sales) * sum(last.sales) （计算结果不超过 20）
        20 （否则）

加起来就得到 MPI 总和了：

    mpi =
        mpi_a + mpi_b + mpi_c + mpi_d + mpi_e + mpi_f

4 决策
---

### 4.1 快速决策流程

MESE 并不存在唯一正确的决策流程。考虑到比赛形式、时间限制等因素，不同赛事中的决策方式会很不一样。下面介绍一套简单、易于上手的决策流程，适用于单人、三到五分钟的快速决策。

拿到一张报表时，应从上一期的销售情况看起，先查看公司的存货和 UFO（Unfilled Orders）。在没有囤货计划的情况下，如果有超过产量 15% 的存货或超过产量 5% 的 UFO，意味着之前对市场形势的判断很可能已经失准。但也有例外，例如有玩家做出反常的决策，或自己恰好是市场上唯一投入 Mk 的公司，那么出现大量存货或 UFO 并不奇怪。因此，在看了存货和 UFO 之后可以接着看玩家栏中的情况，尤其要关注两类人，其一是自己主要的对手，其二是有数据异于寻常的“搅局者”。

接下来，如果可用的现金和贷款限额有限，需要计算自己的可用资金。根据之前 loan_early 的计算公式可知，可用资金为：

    avaliable_fund =
        last.cash + loan_limit - last.loan + deprecation

需要注意，可用资金中可以额外加上一份折旧。一个推测是，MESE 原本的设计是不允许产能减少的，即 CI 的值不能小于折旧，但由于种种原因修改成了现在这样。

一般来说，前几期可用资金较为紧张，需要充分利用。在所有决策中，可以先确定的是开工率。通常前期的开工率都在 85% 到 95% 之间，低于 80% 的开工率只会出现在少数极端局面中。产量为开工率乘以产能，计算即可。然后，初步判断 Mk 的效果。观察玩家栏，如果销售额高的公司明显利润更高，那么 Mk 效果更有可能是好的。可以再判断其它公司在新的一期 Mk 决策会如何变化，据此决定自己是否投入 Mk。需要注意，由于 Mk 具有竞争性，如果大量公司都打算投入 Mk，则 Mk 的效果就会变差，因此预判其他玩家的决策趋势也很重要。最后，综合考虑本期及之后一期产能和研发的重要性，将剩余的资金分配给 CI 和 RD。如果已经有较多的产能或存货，资金分配可以更倾向于 RD，反之倾向于 CI。

在资金充足时，以上几项决策可以分开考虑。开工率在利润丰厚、产能不足时可适当提高，反之减少，直到达到 80% 和 85% 之间。要注意边际成本应该低于价格，通常控制在价格的三分之一至二分之一左右。Mk 可以根据效果好坏投入一个极大的值，或不投。在玩家总数较少时，即使 Mk 效果不好，也可以适当投入，以避免一家或两家独占份额。在总产能较少时，CI 通常可以投满，但出现产能过剩、存货累积的趋势时，应及时削减至与折旧接近。RD 应该先尽可能大量地投入，然后根据自己的战略和市场的长期情形来决定一个计划上限，投满后就停下。考虑到 RD 的作用方式，越早投 RD 越有利，例如七期的比赛中应尽量在前四期投完计划中的 RD，之后就不应继续投入 RD。

价格是最后确定的决策。多数情况下，定价的目标是使供需平衡，即既不产生过多存货，也尽量避免 UFO 的出现。

定价的第一步是预测市场走势。市场走势指在市场上可获得利益的大小，需要注意，除了报表中的利润，RD 本身也是有价值的。因此，分析市场走势时需要在利润上加上部分当期 RD，或者在销售额上减去部分当期 Mk 和每期平均 RD。通常来说，市场的变化与所有玩家每期平均 RD 的关系最为紧密。前期市场会快速增长，而后期大部分玩家停止投入 RD 后，市场会由盛转衰。此外，市场上存货和 UFO（可以用订单总量减去总销量得到）的情况也可以辅助判断，大量 UFO 意味着市场好于大多数玩家的预期，而大量存货相反。

为方便计算，我们以销售额为基础，来应用预测结果。结合对市场走势的判断，以及上一期的数据，我们可以初步预估自己在决策大体不变的情况下可以获得的销售额。然后，可以在此基础上，根据本期决策的变化，调整销售额预期。例如本期比上期多投入 5000 的 Mk，则销售额预期应提高 5000 或更多。反之，若少投入 5000 的 Mk，则销售额预期应降低 5000 或更少。RD 的效果可以使用类似 Mk 的方式来预估，但应采用每期 RD 平均值，而非本期 RD 决策。

最后，将调整后的销售额预期除以产量与存货之和，得到一个预估的平衡价格。可以在此基础上稍稍调高价格决策，以避免 UFO。需要注意，40 是一个特殊的价格分界线。在得到价格决策后，如果其远高于 40，则应在预测基础上适当降低价格相比上期的变动幅度（无论是加还是减），而如果只是稍高于 40，则不需要太多调整。而在 40 以下的低价阶段，应该更积极地控制成本、减小投入，争取在价格战中取得主动，或者应用“反弹”一类的战术寻求盈利机会。后文对反弹会进一步讲解。

### 4.2 宏观与战略

每场 MESE 比赛的风格由两个因素奠定，其一是参数，其二是其他玩家的决策。一些赛事中的参数是已知的，另一些赛事则需要玩家通过解读文字提示来推测参数。而其他玩家的决策主要通过逆向分析（“跟踪”），结合对他人决策风格的判断得到。

参数对整个市场会有许多影响，我们通常会关注市场需求、决策权重以及资金设定。

市场需求主要由 demand 设定控制，也通常是宏观信息中最常见、最容易解读的部分，但由于玩家的决策不同，不同局中的市场变化方式也会有一定差异。在 RD 的推动下，默认设定对应的市场是先增长后衰减的，呈现倒抛物线形。如果其中有反常之处，就有可能是参数的影响。

决策权重对应 share，即价格、Mk、RD 对订单的影响能力。在常见的设定中，343 一般被认为是稍重 Mk 和 RD 的，经常会导致高投入、高利润的局面，而 262 是稍重价格的，对降价过程的精准性要求更高。MESE 默认的 15% : 70% : 15% 的 share 比例下，价格的效果是十分显著的，市场会很快进入低利润阶段。

资金设定也会显著地改变局面，尤其是贷款限额。较少的可用资金意味着玩家的投资会减少，市场会相应缩减，这样的局面下更有可能出现极端而非中庸的决策。Mk、CI 和 RD 的上限也能起到改变市场走势的作用，但对决策差异性的影响却与贷款限额相反，例如决策上限小于 10000 的 Titan 会比 MESE 更倾向于细节比拼。税率有时也会发挥作用，例如可以选择税率高的期数来投入 RD 或适当囤货。

MESE 一大吸引人之处在于，它具有“少数占优”的原则，与众不同的决策往往能获得优势，这就带来了博弈的乐趣。价格、Mk 和 RD 都具有竞争性，因此最优的决策往往会落在几个截然不同的点上。

RD 是 MESE 中与战略关联最紧密的决策，通常我们把决策风格分成超轻 RD（“裸奔”）、轻 RD、中 RD、重 RD 和超重 RD 五档。在七或八期、八玩家的标准局中，它们分别对应约 15000 以下、15000 至 25000、25000 至 35000、35000 至 45000、45000 以上的累计 RD。

超轻 RD 通常对应的策略是前期快速获得利润，而中后期领先降价。超轻 RD 玩家有时需要舍弃利润，主动降价，来拉低整个市场的利润空间，防止被 RD 较高的玩家追上。

轻、中、重 RD 是主流的决策风格，打法是前期累积 RD，中期放 RD 并赚取利润，后期通过比拼细节来攻防。RD 的投入量要根据对市场走势的预判来选择，市场衰落越快，越少的 RD 占优，反之越多的 RD 占优。对于主流 RD 量的决策，Mk 的配合也是非常重要的，通常市场较好、自己的 RD 越多时，投入 Mk 越有可能有利。

超重 RD 是较为反常识的决策方式，与重 RD 相反，它适合于很早衰落的市场。超重 RD 主要的优势来自少数占优，即其他玩家因为市场不佳或参数限制，RD 投入明显较少，导致一人独得可观的 RD 份额。超重 RD 经常与后期的反弹战术结合。

Mk 与价格通常是共同配合的，当利润空间较大时，高价格、高 Mk 经常出现，反之则会有大量的低价格、低 Mk 的决策。但由于少数占优，在玩家的 Mk 决策趋同时，少数派会取得优势。例如当整个市场普遍资金紧张时，市场总 Mk 就会较少，此时投入 Mk 虽然会牺牲其它决策，但可能有意想不到的效果。同样，当大量玩家同时堆起 Mk 时，放 Mk 而降价的玩家能省去大量花费，取得较高的利润。

另外，需要注意一个细节。MESE-Next 中无论实际玩家数多少，都是按照八玩家的手感来设置参数的。但在 MESE 和 Titan 中，若不是八玩家，需要将各种总额、限额等数字除以八并乘以玩家数，才能按照八玩家的经验来操作。例如六玩家 20000 的决策上限，与八玩家 15000 的决策上限是对应的。

### 4.3 具体战术

MESE 中，随着市场的变化，前期和中后期的战术呈现不同的形态。前期主要的关注点主要在战略定位，以及对有限的资源的利用上，而后期更偏向于根据定位进行攻防，以及对细节的把握。

首先，关于第一期。由于信息有限，第一期的决策一般基于固定的模板，根据宏观信息以及对其他玩家的了解微调得到。MESE 中常见的起始价格是 65 到 80 之间，Titan 中稍高。对于 Mk，由于首期利润预期低，投入高 Mk 是比较冒险的，但为了避免一家独得，可以适当投入。而对于 RD，由于其越早投入效果越好，即使决定裸奔也可以投一些，来减轻开局失利的风险。第一期的资金不算太紧张，除非打算积累极高的 RD，否则剩余资金应投给 CI。

在常见的设定下，第二、三期往往是可用资金较为紧张的阶段，有两种经典战术可以应用于此。一种战术称为“机械推进”，无论局面如何，都强行投入较高的 RD，以换取中期的主动权。另一种战术是趁所有玩家资金不足时投入高 Mk，争取独占大部分 Mk 份额。这通常需要在前一轮以存货或者产能作为铺垫。

### 4.4 团队赛事策略

5 高级话题
---
