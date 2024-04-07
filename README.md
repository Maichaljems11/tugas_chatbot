def chatbot_response(message):
    message = message.lower()

    if message == 'hallo':
        return 'Hai, ada yang bisa saya bantu?'

    elif message == 'bagaimana kabarmu?':
        return 'Saya baik-baik saja, terima kasih sudah bertanya!'

    elif message == 'sampai jumpa':
        return 'Sampai jumpa lagi!'

    else:
        return 'Maaf, saya tidak memahami pesan Anda.'

print('Chatbot sederhana: (Ketik "sampai jumpa" untuk mengakhiri)')
while True:
    message = input('Anda: ')
    if message == 'sampai jumpa':
        print('Chatbot: Sampai jumpa lagi!')
        break
    else:
        print('Chatbot:', chatbot_response(message))
