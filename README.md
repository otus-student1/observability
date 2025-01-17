# observability

В проект добавлен docker-compose для запуска Grafana. Заместо alertmanager использован mimir, так же были созданы директории data и provisioning для хранения данных, генерируемых Grafana. Переменные окружения настроены и добавлены. 
1. В интерфейсе Grafana были созданы две папки:app и infra(1)
2. Добавлен источник данных mimir(2)
3. Для папки infra из grafana.com/grafana/dashboards был подключен дашборд для Node Exporter, предназначенный для мониторинга состояния(3)
4. Для папки app подключен дашборд для Blackbox Exporter(4)
5. Для папки infra также были добавлены метрики для MySQL, скачанные с того же ресурса(5)