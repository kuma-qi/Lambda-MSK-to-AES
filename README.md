# Lambda-MSK-to-AES
use lambda wirte data from Amazon MSK(kafka) to Amazon ElasticSearch（Opensearch）
kafka是常见的数据管道，ES是常见的数据分析，kafka到ES的数据打通是常见的需求，常见的有几种方法:
* 使用logstash kafka插件;
* 使用kafka Connect通过Jest实现Kafka对接Elasticsearch;
* 自写程序读取、解析、写入。

前两种方法在托管的服务中通常是没法实现的，那么我们今天就通过使用lambda，通过代码的方式，只需修改相应参数，就可以快速的帮助MSK和AES的用户快速实现数据对接。

本脚本需要对lambda有一定使用基础，如果您不太了解lambda请看这篇：  https://github.com/aws-samples/amazon-elasticsearch-lambda-samples  

