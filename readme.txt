1. mkdir learngit //�½��ļ���
2. cd learngit //�����ļ���
3. pwd // �鿴�ļ���·��
4. git init // �����Ŀ¼���git���Թ���Ĳֿ�
5. Ȼ������½�readme.txt����д����
6. git add readme.txt // ���ļ���ӵ��ֿ� 
    git add .  // �������ļ���ӵ��ֿ�
7. git commit -m "wrote a readme file" // ���ļ��ύ���ֿ�
8. git remote add origin https://github.com/chenrunmiao/learngit.git
9. git push -u origin master // �ᱨȨ�޴���
	git@github.com: Permission denied (publickey).
	fatal: Could not read from remote repository.
	Please make sure you have the correct access rightsand the repository 	exists.
���������ɾ����ǰkey����������key
1. ssh-keygen -t rsa -C "githubע������"
2. ֱ�ӻس�Ĭ��
3. Ȼ���C:\Users\Administrator\.ssh�����id_rsa.pub
4.��github����¼�����˻������Ͻ�settings ���� SSH and GPG keys ���� New SSH key
5. title���д��key��id_rsa.pub���ƽ�ȥ
6. git push -u origin master  // �ɹ���

�ϴ��ļ���github��
1. git add .   // ��ӵ����زֿ�
2. git commit -m '����'  // ����ύ����
3. git pull origin master  // �ύǰ�ȴ�Զ�����ֿ�����ȡ����
4. git push -u origin master  // �ѱ��زֿ�����ύ