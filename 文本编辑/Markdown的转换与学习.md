# Markdown��ת����ѧϰ

������Ҫ�ֳ��Ĳ��֣���һ����Markdown��Latex�ļ���ת�����ڶ����ֹ���Markdown��֪�����µ�ת���������������������漰ת�������Σ����Ĳ����ṩһЩѧϰMarkdown�Ĳ��ϡ�

## Markdown��Latex�ļ���ת��

Markdown�﷨��Լ򵥣�������ʱ�༭����ʱ��Ⱦ����Latex�������趨�����õ�packages�Ͱ�ʽ����Ը��ӡ����Markdown�����ڷ��㼰ʱ�ļ�¼����Latex�����ڽ�Ϊ��ʽ�Ĳ��ϵı༭�������ģ��̲ĵȡ���ʱ������Ҫ��һ��Markdown���ݲ���Latex�У���Latex�е�һ�ε���ΪMarkdown����������ȽϺý����

�����Ϊ����Ƽ�һ��Markdown�༭����Typora��[����](https://typora.io/)����Ϊ��ʹ��ת�����ܣ�������Ҫ��װPandoc������һ��Github�ϵĿ�Դ��������ǿ���ͨ�������������Ҳ������Typora�İ����˵���ѡ��Install and Use Pandoc��ȡ����������ַ��[����](https://github.com/jgm/pandoc/releases/tag/2.10.1)������װ��ɺ� ���ǾͿ���ʹ���ļ��˵��еĵ���͵������ܶ�ȡ�ͱ���ΪLatex�ļ��ˡ�

## Markdown��֪����ת��

�ܶ��˸�ϰ����Markdown�������н��б༭����ϰ����֪�����ڽ��б༭������֪���༭�����ݽ϶�ʱ���ܳ��ֿ������⣬��˽���Markdown�༭֪��������ش�ͳ�Ϊ�����⡣������������д���֣���������ҵķ�������Ҳο���

�������ϴ�֪������ʱ��֪������ʹ��Markdown�﷨������Ҫת������ʹ�õ�������Markdown�༭����mdnice��[����](https://www.mdnice.com/)����������Ҫ�ѱ༭�õ��ĵ����Ƶ�������������Ͻǵİ�ť�����ɸ��Ƶ�֪����΢�Ź��ں��ˣ�ͼƬ�������赥������������Դ˷��������⣬�ҿ���Ϊ���ṩһЩ����˼·��

[˼·һ](https://zhuanlan.zhihu.com/p/91887957)��[˼·��](https://zhuanlan.zhihu.com/p/97455277)��[˼·��](https://zhuanlan.zhihu.com/p/99057715)��[˼·��](https://zhuanlan.zhihu.com/p/141590985)��

���ǿ���д��һЩ֪����ϣ�����ر����������ҵ��������£�

���ȣ������µײ�������ã��޸����£�����༭ģʽ��Ȼ��ճ�����հ׵�Typora�У����档ʹ������python���봦�����md�ļ���

```
import re
raw_file="name1.md"  #������ת�����ļ���
made_file="name2.md"     #��ת������ļ�����
with open(raw_file,"r",encoding="utf8") as f:
    s = f.read()
t = re.sub(r"\!\[(.*)\]\(.*?\)\1",r"$\1$",s)
with open(made_file,"w") as f:
    f.write(t)
```

������ת������ļ�������ȷ��Markdown�ˡ�

ע����������������֪�����⣺[����](https://www.zhihu.com/question/309343971/answer/959074405?utm_source=wechat_session&utm_medium=social&utm_oi=925517376135499776&utm_content=group3_Answer&utm_campaign=shareopn)����л֪���û��� [@��ʿͯ](https://zhuanlan.zhihu.com/people/1756465d35cf4b6ec1c6df040d98d214) ��

��������Ҫ�����ǿ��Ա༭���£��������������Լ������ģ���������˵����£��Ҳ�û���ҵ��Ϻõİ취�������еĹ�ʽ����ʽ����ͼƬ���ֵģ����ǲ�����༭ģʽֱ�Ӹ��Ƶõ��Ĺ�ʽ������һ������ַ�����ӣ��ò�����ʽ���ݣ�����������ܿ��е�˼·��

[˼·һ](https://zhuanlan.zhihu.com/p/56694990)��[˼·��](https://zhuanlan.zhihu.com/p/110250329)��[˼·��](https://zhuanlan.zhihu.com/p/29778024)��

## ����ת��������

���Ǵ�Typora�ĵ����뵼���˵������Է��֣���������֧����Latex�ļ���ת������֧��������һЩ��ʽ�����ǱȽϹ�עWord��Epub��Pdf������ζ�ţ�Markdown�ļ�������Word�޷��л���

Ȼ��������ֻ�������Pdf�������Ե���Pdf�����ǣ��������õ�һƪ���ĵ�Pdfʱ�����ǿ����Ƚ�Pdfת��ΪEpub���ٵ���Epub���õ�Markdown���롣��ˣ�Markdown�ǿ�����Pdf�ĵ���ת�ģ�ǰ����Pdf�����Markdown���루Ӱӡ������Pdf���������ת������

���⣬����Pdfֱ��תMarkdown�Ĺ��ߣ���ַ��https://pdf2md.morethan.io/

�����ַ�������⣺

[��û��ʲô�취��pdfת��markdown��](https://www.zhihu.com/question/300833276/answer/1230291158?utm_source=wechat_session&utm_medium=social&utm_oi=925517376135499776&utm_content=group3_Answer&utm_campaign=shareopn)

## Markdownѧϰ����

1��https://blog.csdn.net/qq_30241709/article/details/88654050 

2��https://www.jianshu.com/p/5a27d195678f 

3��[blog.csdn.net/apr15/article/details/105597907?utm_medium=distribute.pc_relevant.none-task-blog-title-2&spm=1001.2101.3001.4242](https://blog.csdn.net/apr15/article/details/105597907?utm_medium=distribute.pc_relevant.none-task-blog-title-2&spm=1001.2101.3001.4242) 

4��https://blog.csdn.net/young951023/article/details/79601664?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-1.nonecase&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-1.nonecase 

5��https://www.jianshu.com/p/7c34f5099b7e

�Ҹ������ϼ�������������һ�����Լ�����ѧ��ʽ�б������ڱ�ר����Github��Ŀ�ϡ�

[DSroad](https://github.com/ButterYan/DSroad)

��Ȩ˵�������ַ�����֪�����ѱ������ἰ�����޷���֤��¼��ȫ��������ṩ��Դ��������⡣