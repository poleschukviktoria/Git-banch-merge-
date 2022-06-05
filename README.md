# GitHub. HW_2
1. На локальном репозитории сделать ветки для:  
- Postman
- Jmeter
- CheckLists
- Bug Reports
- SQL
- Charles
- Mobile testing

>git branch Postman  
>git branch Jmeter  
>git branch CheckLists  
>git branch BugReports    
>git branch SQL    
>git branch Charles  
>git branch MobileTesting  

2. Запушить все ветки на внешний репозиторий  
>git push origin --all  

3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта  
>git checkout BugReports  
>cat >> BugReport.txt  
```html
ID:
Title:
Environment:
Precondition:
Data:
STR:	
AR:
ER:	
Attachments:
Severity (Blocker, Critical, Major, Minor, Trivial):
Priority (High, Medium, Low):
```  
>Нажать Ctrl+D  

4. Запушить структуру багрепорта на внешний репозиторий  
>git add .  
>git commit -m "add Bagreport.txt"   
>git push --set-upstream origin BugReports  

5. Вмержить ветку Bug Reports в Main  
>git checkout main  
>git merge BugReports -m "merge BugReports"  

6. Запушить main на внешний репозиторий.  
>git push  

7. В ветке CheckLists набросать структуру чек листа.  
>git checkout CheckLists  
>cat >> CheckList.txt  
```html
id:
Summary:
Result:
Status (passed, failed, blocked):
```
>Нажать Ctrl+D  

8. Запушить структуру на внешний репозиторий  
>git add .  
>git commit -m "add CheckList.txt"  
>git push --set-upstream origin CheckLists  

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main  
>нажать Pull Request в GitHub  
>выбрать ветку CheckLists в main  
>Create pull request  
>Merge pull request  
>Confirm merge  
>Create a merge commit  

10. Синхронизировать Внешнюю и Локальную ветки Main  
>git fetch  
>git pull  
