import telebot

TOKEN = 'حط_التوكن_بتاعك_هنا' 
bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "أهلاً بيك! أنا بوت شغال 100% 🔥\nاكتبلي أي حاجة هرد عليك")

@bot.message_handler(func=lambda m: True)
def echo
