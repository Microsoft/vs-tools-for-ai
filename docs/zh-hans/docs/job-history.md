# 查看最近任务的性能和详情

任务一旦提交后，可以在任务列表里看到它们的状态，运行时间和更多信息。

1. 在**服务器资源管理器**展开到某个计算环境。 
2. 双击**Jobs**。
3. 可以看到已经提交到这个计算环境的所有任务。 
4. 在列表中选择某个**job**来查看详情。

![监控任务](./media/monitor-jobs.png)

> 提交到Linux虚拟机中的任务历史存放在虚拟机的/tmp目录中。 因此，当计算机重启后，任务历史会被清除。 要持久保存任务历史记录，请将虚拟机配置为Azure Machine Learning中的计算环境，然后将任务提交到Azure Machine Learning（将虚拟机选为计算环境）。