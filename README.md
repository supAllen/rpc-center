# rpc-center
服务发现

1、zk服务注册，包括多实例注册
    
    Consul 思考

2、服务状态感知

    临时结点+长连接
    主动下线+心跳检测
    
3、实现几种高可用方案

    Failfast
        正常实现，直接抛错
        
    Failover
        出错，调用其他结点
        
    Failtry
        当前结点尝试
        
    Failbackup
        当前结点一定时间内不返回结果则异步请求其他结点
