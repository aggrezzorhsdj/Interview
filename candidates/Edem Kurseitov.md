
# Отличие sessionStorage от localstorage

Основное отличие между `localStorage`, `sessionStorage` и cookies заключается в сроке хранения данных и области видимости. `localStorage` хранит данные бессрочно (пока не удалены вручную), `sessionStorage` - только в рамках текущей сессии (до закрытия вкладки), а cookies - это небольшой фрагмент данных, который может быть отправлен на сервер с каждым запросом и имеет свой срок жизни, который задается при создании. 
Подробнее:

- **localStorage:**
    
    - Данные хранятся неограниченное время, пока пользователь их не удалит (например, через очистку кэша браузера). 
    - Данные доступны для всех вкладок и окон браузера с тем же источником. 
    - Идеально подходит для хранения настроек пользователя, данных профиля и другой информации, которая должна сохраняться между сессиями. 
    
- **sessionStorage:**
    
    - Данные хранятся только в течение текущей сессии браузера (до закрытия вкладки или окна). 
    - Данные доступны только для текущей вкладки (контекста). 
    - Подходит для хранения данных, связанных с текущим взаимодействием пользователя с сайтом, например, данных формы. 
    
**Cookie storage** — это способ хранения небольших текстовых файлов (куки) на устройстве пользователя браузером, которые содержат данные о сеансе и пользовательских настройках. Основные характеристики cookies:

- Хранятся в браузере и автоматически отправляются на сервер с каждым HTTP-запросом к соответствующему домену.
- Объем ограничен примерно 4 КБ.
- Срок хранения задается при создании и может быть как сеансовым (удаляется после закрытия браузера), так и постоянным.
- Используются для управления сессиями (авторизация), персонализации и трекинга.
- Могут быть защищёнными, чтобы скрыть содержимое от клиента (например, для токенов аутентификации).
    

Cookies удобны для идентификации пользователя и передачи данных на сервер, но имеют ограничения по объему и безопасности, а также увеличивают сетевой трафик из-за передачи с каждым запросомtorage ?

# Как синхронизация вкладок работала через BroadcastChannel API?

# Зачем wasm что за вычисления?

# Какой самый большой и сложный модуль/компонент реализовал?

# Про библиотеку UI kit 

3 аппликейшена использовали либу в виде нмп пакета?