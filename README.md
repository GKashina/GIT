1. На локальном репозитории сделать ветки для:
- Postman		git branch Postman
- Jmeter 		git branch Jmeter 
- CheckLists		git branch CheckLists
- Bag Reports		git branch Bag Reports
- SQL			git branch SQL
- Charles		git branch Charles
- Mobile testing	git branch Mobile testing

2. Запушить все ветки на внешний репозиторий 
	git push origin --all

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта 
	git checkout Bag Reports
	cat > bug_report.txt
ID
Severity
Priority
Title
Precondition
Environment
Expected result
Actual result
Attachments
Postcondition

4. Запушить структуру багрепорта на внешний репозиторий
	git add .
	git commit -m "added bug_report.txt"
	git push

5. Вмержить ветку Bag Reports в Main
	git checkout main
	git merge Bag_Reports
6. Запушить main на внешний репозиторий.
	git push
7. В ветке CheckLists набросать структуру чек листа.

ID
Severity
Priority
Title
Precondition
Environment
Expected result
Actual result
Attachments
Postcondition

8. Запушить структуру на внешний репозиторий
	git add .
	git commit -m "added checklist.txt"
	git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
	На внешнем репозитории сделать pull request
Compare & pull request
Create pull request
Merge pull request
Confirm merge 

10. Синхронизировать Внешнюю и Локальную ветки Main
	git pull
