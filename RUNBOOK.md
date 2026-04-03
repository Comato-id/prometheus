# RUNBOOK

## 1. Node Exporter
Установить node-exporter на сервера CA и VPN.
Создать systemd unit.

## 2. OpenVPN Exporter
Установить exporter на server-vpn.

## 3. Prometheus
Установить Prometheus.
Настроить prometheus.yml.
Создать systemd unit.

## 4. Alertmanager
Настроить alertmanager.yml.
Добавить email уведомления.

## 5. Alerts
Создать файл alerts.yml.

## 6. Интеграция
Подключить alerts.yml в prometheus.yml.

## 7. Безопасность
Настроить iptables.
Ограничить SSH доступ.

## 8. Telegram
Создать бота и подключить webhook.
