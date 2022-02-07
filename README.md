# my-flink-cdc-stream

1.目前接了MySQL source ,sink为steam可自定义输出数据源，可追踪MySQL的binlog监听获取表数据变化

2. op=c表示 insert/creat 操作；op=d表示 delete；op=u 表述 update

3.当前重启不能获取历史操作，只能获取当前表截面数据，且op=r/read

todo:重启应该衔接上次服务关闭时的操作
