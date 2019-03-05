对象
======
Context (策略信息总览, 包含账户,时间等信息)
-------
>   subportfolios : 当前单个操作仓位的资金,标的信息, 是一个 SubPortfolio 的数组
>   portfolio : 账户信息, 即 subportfolios 的汇总信息, Portfolio 对象
>   current_dt : 当前单位时间的开始时间 , datetime.datetime 对象
>   previous_date : 前一个交易日 , datetime.date 对象.
>   run_params: 此次运行的参数:
>       start_date :  回测/模拟开始日期, datetime.date对象
>       end_date : 回测/模拟结束日期, datetime.date 对象
>       type : 运行方式 : 'simple_backtest':通过点击 '编译运行' 运行;   'full_backtest': 通过点击 '运行回测' 运行; 'sim_trade' : 模拟交易 ; 'live_trade': 实盘交易
>       frequency: 运行频率,  'day', 'minute', 'tick'

SubPortfolio  (子账户信息)
---------
