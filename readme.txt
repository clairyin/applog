��¼˵����
1.���ݿⶼ�����ҵĿ�������
  192.168.190.29
  mysql -uroot -p -h192.168.190.29 --auto-rehash

  ��Ʒ�����applog���ݿ�ṹ:applog
    (app-->version-->module-->page-->action)
  �������applog���ݿ���ȡ���ݵ�autoapplog
    (define_action)

select  id, version_num, app_id, app_type ,status ,create_time, update_time from applog_version;
select * from applog_action where action_code ='2-100004';
select * from  define_action limit 1;

����define_action������ֶ�������ʾ�Ƿ�Ϊ�������߱༭����

id��ȡapp+version   

