---
name: 常见问题  
---

# 常见问题   NO

### 如何使用 NGINX 进行反向代理？

下面是一个 NGINX 的示例配置分区，但需要注意值可能和实际情况有所不同： 

```nginx
server {
	listen 80;
	server_name peachdocs.org;
	
	location / {
		proxy_pass http://localhost:5556;
	}
}
```

### 自定义目录必须是一个 Git 仓库吗？

不是的，自定义目录可以只是一个普通的目录。但一般推荐将它保存为一个 Git 仓库以方便同步和备份。
