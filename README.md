package SQL;

public class SOLdatestyle {
   /**
    * 数据库
    *     存储数据的几大类型
    *       Number（参数1，参数2） 参数1表示可以存最大参数1个字符，其中包含参数二个精度
    *       Char(参数A)  参数A表示能存参数A个字节，返回的是字符串，缺点是直接生成参数A个字节不管内容够不够
    *       VarChar(参数1)参数1表示可以存参数1个字节，内容不足参数1个自动缩减，比较耗性能
    *       ORCAL  内有VARCHAR2，功能同VARCHA相同
    *       Date默认格式是DD-MON-RR
    *       
    *       
    *       DEFAULT关键字
    *           放在类型参数后，表示默认值，可以被改变
    *           在数据库中，字符串用‘ ’表示  而Java是 b'n“”表示字符串，，如果没有DEFAULT那么没有传的话默认是null
    *       例如：name CHAR(30) DEFAULT '小红'
    *       
    *       NOT NULL是一种约束条件，是必填项
    *       例如：name CHAR(20) NOT NULL----表示这一列必须给定值
    *       
    *       DDL---新建表
    *       DML---增删改表
    *       TCL---事件控制
    *       DQL--数据查询语句
    *       DCL--数据控制，指定用户授权
    * 
    * 
    * 
    * 数据库中写表
    * CREATE TABLE [可以不写，这里指定向]  表名（
    *                       字段名 NUMBER(4),
    *                       字段名 CHAR(70),
    *                       字段名 VARCHAR(50),
    *                       字段名 VAR
    *                       字段名 DATE
    * ）
    *  
    *  DESC 表名----查看表结构，包括列的名字，类型，长度等
    *     例如DESC file
    *     
    *  DROP TABLE 表名字-----删除表
    *  
    *  RENAME 表名 TO 新表名-----重新给表命名
    *  
    *  ALTER TABLE 表名 ADD (字段名 NUMBER(6) NOT NULL,.......)----追加新列
    *  
    *  ALTER TABLE DROP(列名字)-----删除列
    *  
    *  ALTER TABLE 表名 MODIFY (字段名 NUMBER(20))-----修改一列的列名字，一般类型不变，只影响以后插入的数据
    *  
    *  
    *  DML伴随着TCL事物控制语言搭配使用
    *  
    *  INSERT INTO 表名[(列名1,列名2)] VALUES(列1值，列2值)------向列名1和列名2中插入 列值，表名表值一一对应，没有的列明插入null
    *  
    *  SELECT * FROM 表名-----查询表名中的数据
    *  
    *  
    *  COMMIT----提交SQL语句，将缓存在SQL DEVELOPMENT 的内容写入数据库中
    *  
    *  ROLLBACK-----回滚将还在缓存的没有提交的内容全部清除
    *  
    *  TO_DATE(参数1，参数2) ----参数1是日期，参数2是格式，例如YYYY-MM-DD年-月-日。TO_DATE是函数，返回值是指定格式的日期
    *  
    *  UPDATA 表名 SET 列名1=值1 WHERE 列名2=“值2”-----where是过滤条件，意思是列明2=“值2”的那一行的列名1更改为值1
    *  
    *  DELETE FROM 表名 WHERE  name='小红'-----删除name是小红的的那一行
    */
}
