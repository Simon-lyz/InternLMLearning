# InternLMLearning
### 全链条开放体系 | 部署
1. 大模型特点
   - 内存开销巨大：本身参数量大、采用自回归生成token，需要缓存k/v
   - 动态shape：单个token * length，length不定，请求数不固定
   - 模型结构是Decoder only
![
2. 技术挑战
   - 设备：低存储设备的部署（消费级显卡、移动端）如何部署？
   - 推理：加速token的生成熟读、动态shape的推理、如何有效管理和利用内存
   - 服务：提高整体吞吐量，降低请求的平均响应时间

3. 部署方案
   - 模型并行，低比特量化，Attention优化，计算和访存优化，Continuous Batching
     
### 全链条开放体系 | 智能体
