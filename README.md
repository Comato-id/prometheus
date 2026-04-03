# Prometheus Monitoring Stack
Cистема мониторинга и алертинга на базе Prometheus.
Что реализовано
- Сбор метрик с серверов через Node Exporter
- Мониторинг сервисов (Prometheus targets)
- Алертинг через Alertmanager
- Уведомления:
  - Email (SMTP Gmail)
  - Telegram (через webhook + bot)
- Безопасность:
  - Firewall (iptables)
  
# Архитектура
[Node Exporter] → [Prometheus] → [Alertmanager] → [Telegram / Email]
## 📊 Monitoring

### Prometheus Targets
![Targets](images/prometheus-targets-up.png)

### Telegram Notification
![Telegram](images/telegram-alert.png)

### Email Notification
![Email](images/email-alert.png)
