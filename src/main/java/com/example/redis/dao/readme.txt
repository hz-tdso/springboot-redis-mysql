spring boot整合mybaits，使用mapper（或dao）时需注意：
    ①mapper接口不用添加任何注解
    ②mapper.xml文件中命名空间一定要配成对应mapper接口的全类名
    ③必须在application类上加上@MapperScan("com.example.redis.dao")注解才能保证spring在autowire mapper时能成功