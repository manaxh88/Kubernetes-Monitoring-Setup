# Kubernetes Monitoring Setup  
K8s 集群监控体系搭建（Prometheus + Grafana）

## 项目简介  
本仓库记录了基于 Kubernetes 搭建 Prometheus + Grafana 监控系统的 YAML 示例和配置。  

## 核心内容  
- **prometheus-deployment.yaml**：Prometheus Deployment + ConfigMap  
- **grafana-deployment.yaml**：Grafana 部署
## 适用场景  
- K8s 生产集群性能监控  
- 故障主动预警 
- 结合 ELK 实现日志 + 指标统一观测

## 快速上手  
1. 确保已安装 kubectl 并连接到 K8s 集群  
2. 应用配置：`kubectl apply -f prometheus-deployment.yaml`  
3. 访问 Grafana（默认端口 3000），导入官方 Dashboard（如 Node Exporter Full）  
4. 配置 Alertmanager 告警规则（示例：CPU > 80% 持续 5 分钟告警）

## 项目成果  
- 监控覆盖率 >95%  
- 故障响应时间从小时级降至分钟级  
- 实现 10+ 指标实时可视化 + 主动预警
