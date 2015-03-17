记录说明：
1.数据库都是用我的开发机器
  192.168.190.29
  mysql -uroot -p -h192.168.190.29 --auto-rehash

  产品定义的applog数据库结构:applog
    (app-->version-->module-->page-->action)
  从上面的applog数据库拉取数据到autoapplog
    (define_action)

select  id, version_num, app_id, app_type ,status ,create_time, update_time from applog_version;
select * from applog_action where action_code ='2-100004';
select * from  define_action limit 1;

需求：define_action中添加字段用来显示是否为新增或者编辑过的

id获取app+version   

