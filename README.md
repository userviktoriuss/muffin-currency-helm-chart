# Helm-чарт для проекта muffin-currency

Необходимо создать helm-чарт, воспроизводящий логику [этого манифеста](https://raw.githubusercontent.com/adan1lov/muffin-currency/refs/heads/main/k8s.yaml)

N.B.: заменил контейнер в манифесте на свой, собранный под arm.

## Что сделано?

1. Сгенерировал чарт с помощью `helm create muffin-currency muffin-currency-chart`
2. Поправил файлы под задание, убрал лишнее
3. Поправил ошибки с помощью `helm template muffin-currency-chart`
4. Создал релиз: `helm create muffin-currency muffin-currency-chart`
5. Посмотрел статус выкатки: `helm list`. Также глянул `kubectl rollout history deployment/muffin-currency-muffin-currency-chart`.

Круто, работает =)
