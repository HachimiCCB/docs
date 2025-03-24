# 东方夜雀食堂 Wiki API 设计文档

## 在线预览
https://dm7m2v24p4.apifox.cn/

## 资源关系
- **食材/料理/酒水** 通过`category`字段进行分类关联
- **料理配方** 作为食材的子关系（嵌套数据`ingredients`数组）
- **顾客偏好** 通过`liked_recipe_tags`和`liked_drink_tags`关联料理和酒水标签

## 通用模式
1. **数据结构复用**：
   - 所有资源共用`id/name/description`基础字段
   - 分页响应统一包含`total/page/limit`元数据

2. **错误处理**：
```json
{
  "error": "INVALID_REQUEST",
  "message": "参数校验失败",
  "statusCode": 400
}

## 特色功能
1. **全局搜索**：
   - 支持跨资源（食材/料理/酒水/顾客）联合搜索
   - 返回精简数据结构
2. **顾客系统**：
   - 完整偏好标签体系（喜欢/讨厌的料理和酒水类型）
   - 出现位置和消费能力数据

## 开发工具
- Apifox：在线文档与测试

- OpenAPI Generator：支持生成TypeScript客户端

- Mock服务：所有接口已配置示例数据