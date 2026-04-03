# Prometheus Monitoring Stack

Система мониторинга и алертинга серверов OpenVPN и CA на базе Prometheus.
Все серверы настроены в YandexCloud, Ubuntu 20.

## Что реализовано

- Сбор метрик с серверов через Node Exporter
- Мониторинг сервисов (Prometheus targets)
- Алертинг через Alertmanager

### Уведомления
- Email (SMTP Gmail)
- Telegram (webhook + bot)

### Безопасность
- Firewall (iptables)
  
# Архитектура
[Node Exporter] → [Prometheus] → [Alertmanager] → [Telegram / Email]
## Monitoring

## Тестирование

Для проверки алертов:
- остановить сервис (например node-exporter)
- убедиться, что алерт перешёл в firing
- проверить уведомления (Telegram / Email)

### Prometheus Targets
![Targets](images/prometheus-targets-up.png)

### Telegram Notification
![Telegram](images/telegram-alert.png)

### Email Notification
![Email](images/email-alert.png)
