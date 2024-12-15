from telegram import Update
from telegram.ext import Updater, CommandHandler, CallbackContext

# /start buyrug'ini ishlash
def start(update: Update, context: CallbackContext) -> None:
    update.message.reply_text("Salom! Men sizning Telegram botingizman!")

# /help buyrug'ini ishlash
def help_command(update: Update, context: CallbackContext) -> None:
    update.message.reply_text("Yordam kerakmi? Bu yerda buyruqlar ro'yxati:\n/start - Botni boshlash\n/help - Yordam olish")

def main():
    # Tokenni kiriting
    updater = Updater("BOT_TOKEN_HERE")

    # Buyruqlarni sozlash
    updater.dispatcher.add_handler(CommandHandler("start", start))
    updater.dispatcher.add_handler(CommandHandler("help", help_command))

    # Botni ishga tushirish
    updater.start_polling()
    updater.idle()

if __name__ == '__main__':
    main()from telegram import Update
from telegram.ext import Updater, CommandHandler, CallbackContext

# /start buyrug'ini ishlash
def start(update: Update, context: CallbackContext) -> None:
    update.message.reply_text("Salom! Men sizning Telegram botingizman!")

# /help buyrug'ini ishlash
def help_command(update: Update, context: CallbackContext) -> None:
    update.message.reply_text("Yordam kerakmi? Bu yerda buyruqlar ro'yxati:\n/start - Botni boshlash\n/help - Yordam olish")

def main():
    # Tokenni kiriting
    updater = Updater("BOT_TOKEN_HERE")

    # Buyruqlarni sozlash
    updater.dispatcher.add_handler(CommandHandler("start", start))
    updater.dispatcher.add_handler(CommandHandler("help", help_command))

    # Botni ishga tushirish
    updater.start_polling()
    updater.idle()

if __name__ == '__main__':
    main()
