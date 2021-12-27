启动sentinel-dashboard   访问:localhost:8080/#/dashboard
逻辑起始 SphU.entry("demo-hello-api") 

默认http拦截器 CommonFilter
注解逻辑: SentinelResourceAspect
sentinel-demo-annotation-spring-aop 启动 调试http://localhost:19966/mytest

spi 责任链
com.alibaba.csp.sentinel.slots.nodeselector.NodeSelectorSlot         DefaultNode
com.alibaba.csp.sentinel.slots.clusterbuilder.ClusterBuilderSlot     ClusterNode
com.alibaba.csp.sentinel.slots.logger.LogSlot
com.alibaba.csp.sentinel.slots.statistic.StatisticSlot
com.alibaba.csp.sentinel.slots.block.authority.AuthoritySlot
com.alibaba.csp.sentinel.slots.system.SystemSlot
com.alibaba.csp.sentinel.slots.block.flow.FlowSlot
com.alibaba.csp.sentinel.slots.block.degrade.DegradeSlot