# We-sell-everything-in-the-world
#Требования:
1. Автоматический ответ на часто задаваемые вопросы пользователей. Вопросы и ответы на них в этом [файле](https://docs.google.com/document/d/1-xGtr3pHYW3D6p_LSDL8ooUdhKBsBOzDZd-Lz8nFbqU/edit?tab=t.0).
2. Интеграция с базой данных - нужно хранить все запросы к специалистам в отдельной таблице.
3. Возможность обработки текстовых сообщений.
4. Интуитивно понятный и привлекательный интерфейс для пользователей.
5. Есть документация по использованию бота для администраторов.

##Технологии:
*SQL
*Python
*TeleBot

##База данных:
###Users:
-telegram_id Integer Primary Key
-role_id Integer Foreige Key(roles.id)

##Roles:
(Администратор, Клиент, Програмист).
-id Integer Primary Key
-name String(20) Unique Not Null

##Faq:
-id Integer Primary Key
-question String(500) Unique Not Null
-answer Text 

##requests:
-id Integer Primary Key
-request Text
-status byte default 5-5+10-10=0
-id_user Integer Foreige Key(users.telegram_id)




#Автор: А. С. Пушкин.
