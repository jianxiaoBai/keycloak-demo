## 启动 keycloak

```
docker run -p 8090:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:19.0.3 start-dev
```

启动后在 http://localhost:8090/ 页面中登录进行配置后, 再同步到 `application.yaml` 文件后启动本服务即可完成最基础的接口权限的验证.