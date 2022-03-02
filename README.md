# fluid_control
npy文件直接使用np.savetxt转成txt文件即可，存放粒子(x,y)坐标 scoop存放勺子的粒子，ball存放小球粒子，fluid存放流体粒子。若为target任务，ballgood存放好球，ballbad为坏球。

target1-3为target任务的3个例子 

fail是target任务的失败例子（捞上黑球）

manually1-2为人工策略2个例子 

meta1-3为使用meta-learning的3个例子 

nometa1-3为不使用meta-learning的3个例子

SPH1-2为迁移到SPH的2个例子

manually例子你在文章中用在target benchmark上，我实验后发现人工策略在target benchmark失败情况主要是捞进黑球。改成solid scoop benchmark或许更好体现预测流体运动的必要性，能成功捞一个小球，但在捞多个小球的时候由于流体的作用无法成功(manually1/Image)。
