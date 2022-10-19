# pre-push-hook
Git hook to prevent push on specific day of week.

# Things you need to do - 
# 1. Copy pre-push file code
# 2. Go to your project/.git/hooks
# 3. Rename pre-push.sample to pre-push
# 4. Paste the above code
# 5. Make this file executable - $ chmod +x .git/hooks/pre-push
# 6. Voila! Now you will see your push is failing when you try to push on Weekends!!

date +%u gives you the day of the week from Monday (1) through to Sunday (7). If it's greater than 5 (Saturday is 6 and Sunday is 7), then it's the weekend.

If you want to restrict developers on other days, change the if condition accordingly. 
