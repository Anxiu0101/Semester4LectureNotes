The content in Lecture-4
## Functional Requirements 

- The statements of services that the system should provide 
- How the system should react to particular inputs 
- How the system should behave in a particular situation 
- Example 1: The User Story Index Card Management system shall provide an export function allowing users to save all index cards in a PDF file
- Example 2: Data scientists and analysts shall be able to perform ad-hoc data analysis through SQL-like queries to find specific data patterns and correlations to improve infrastructure capacity planning

 - 系统应提供的服务声明
 - 系统应如何对特定输入做出反应
 - 系统应在特定情况下如何行事
 - 示例1：用户故事索引卡管理系统应提供导出功能，允许用户将所有索引卡保存在PDF文件中
 - 示例2：数据科学家和分析师应能够通过类似SQL的查询进行临时数据分析，以找到特定的数据模式和相关性，以改善基础架构的能力计划

## Non-functional Requirements 

- The constraints on the services, e.g., timing constraints, resource constraints, constraints imposed by standards
- Example 1: When the system is under peak load, no emergency messages received from the mobile clients shall be dropped, and the cached messages shall be processed as soon as possible and be multicasted to preselected receivers with no further delay.
- Example 2: The system shall collect up to 15,000 even/sec from approximately 300 web servers.

 - 服务的限制，例如定时约束，资源约束，标准施加的约束
 - 示例1：当系统处于峰值负载下时，不得删除从移动客户端接收的紧急消息，并且应尽快处理缓存的消息，并进行多播以预先选择的接收器，而不会进一步延迟。
 - 示例2：该系统应从大约300个Web服务器收集最多15,000/秒。