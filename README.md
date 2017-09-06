# WhatsappShare
first commit

## 两种分享到Whatsapp方式，详细请阅读Demo

### 一、选择分享app
```Intent sendIntent = new Intent();
   sendIntent.setAction(Intent.ACTION_SEND);
   sendIntent.putExtra(Intent.EXTRA_TEXT, "This is my text to send.");
   sendIntent.setType("text/plain");
   startActivity(sendIntent);
   ```
### 二、直接分享到Whatsapp
```Intent sendIntent = new Intent();
   sendIntent.setAction(Intent.ACTION_SEND);
   sendIntent.putExtra(Intent.EXTRA_TEXT, "This is my text to send.");
   sendIntent.setType("text/plain");
   sendIntent.setPackage("com.whatsapp");
   startActivity(sendIntent);
   ```
