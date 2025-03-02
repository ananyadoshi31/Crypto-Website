# Challenges & Solutions

## Challenge 1: Large Coin Images

**Issue:** The API returned **huge logos**, breaking the UI.  
✅ **Solution:**Resized images using **Tailwind CSS**, ultimately removed it since it was not looking appealing.

```javascript
<img src={crypto.image} className="w-10 h-10 rounded-full" />
```
