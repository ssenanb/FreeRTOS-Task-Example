# freeRTOS-Tasks

## 📝 Amaç
Bu proje, STM32 ve FreeRTOS kullanılarak task oluşturma, task parametre gönderimi ve task suspend işlemlerini öğrenmek amacıyla geliştirilmiştir.

## ⚙️ Kullanılan Teknolojiler
- STM32F0 Discovery Board
- STM32CubeIDE
- CMSIS-RTOS v2 (FreeRTOS)
- C (HAL Library)

## 🚦 Yapılanlar
- İki farklı LED task oluşturuldu ve her birine ayrı GPIO port/pin parametreleri gönderildi.
- Bir UART task ile seri port üzerinden index değeri gönderimi yapıldı.
- Belirli koşulda (`task_index == 7`) UART task askıya alındı (`osThreadSuspend`).
- Task'lar arasında bağımsız çalışmayı gösteren temel örnek.

## ❗ Notlar
Bu proje, öğrenme ve deneme amaçlı yazılmıştır. Gerçek uygulamalar için watchdog, error handling ve bellek optimizasyonu gibi ek güvenlik önlemleri gereklidir.
