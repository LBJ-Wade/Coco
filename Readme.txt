Coco��Cosmos cOnstraint COde�����ڶ෽���(��лeasyLTB��CosmoMC��Numerical Recipe)�Ļ�������ɵġ�ּ�ھ����ܼ������Զ��������FRW����£����ʷֲ����ȸ���ͬ�ԣ�������ѧģ�Ͳ��������ƺͻ�contourͼ������
Coco���ص㣺
���԰���ͨ��mcmc����ģʽ��ɻ�contour������
�ṹ��Ȼ�������׶�����
��Ӳ����͹۲����ݼ򵥣�
�����Զ����ɻ�ͼ����IDL�ļ���;
��Linux��Windows�¶����Է��������;
ÿ�����е�ʱ�䣬����ʱ�����õ�ģ�ͺͲ����������������������Ϊinfo.txt���ļ��У�

��Ҫ�����ļ����ܣ�
Coco.f90�ǳ�����ڣ�������ѡ����ʹ����ͨ����(��������㿪��ֵ,use_MCMC=0)����ʹ��MCMC����(use_MCMC=1)��
Settings.f90����������ѧģ�͵ĵط���
ReadInData.f90���������ļ����ߣ����ݵ����ʱ���������ݵ㸳ֵ��������ѡ��ʹ����Щ�۲⣬Ĭ��ʹ�ð���SN��Hz, CMB, BAO��BAOP���ڵ��������ݣ�����ͨ��ֱ��ע�͵��İ취����ĳ�����ݣ��������������ᵼ�½��������޸ģ�
Chi2.f90�������chi square��
ParamScan.f90��use_MCMC��ȡֵ��������ɨ������ռ䣬�����������ʽ�ڲ����ռ����ߣ��õ�һ���ɲ����㹹�ɵ�markov����
GenIDL.f90���ݲ�������ѡ�۲���������һ��IDL�ļ����ڸ��ļ���ʼ����һ��Ŀ¼֮��ֱ�����м��ɵõ�һ�������Ը��������Ƶ�ps�ļ���

���ʹ�ã�
0 �����Զ�����IDL��ͼ�������Ҫ������һ�㣬����Ҫ��װIDL.���õ���IDL 7.1��������Ҫ��������IDL����⣬textoidl�Լ�Coyote(http://www.ast.cam.ac.uk/~vasily/idl.htm)�����������ڵ�λ�������IDL·����
1-Windows
1)��compaq visual fortran��coco.dsw�ļ�(intel visual fortranû�ù�����֪����ô��)��
	�༭coco.f90�ļ���ѡ���Ƿ�ʹ��mcmc������
	�༭readdata.f90�ļ���������ݻ���ע�͵�����Ҫ������(��ReadInObsData�����н��У����磬��ʹ��sn��ע�͵�'call read_sn')��
	�༭settings.f90�ļ�������ģ�ͺͲ������������Ҫ��Щʱ���һ������ļ����������˼���������Ҫ���õı�����
	����io.f90�ļ��е�plotdir�������ɵ����ݺ�idl��ͼ��������������plotdir='D:\'�����ĵĻ�����������coco�ļ��У�
	���룬���У�
2)��idl�����ɵ�.pro�ļ�����LCDM_mcmc.pro��
	����plotdirΪ.pro�ļ�����λ�õľ���·��������plotdir='D:\coco\'
	������ļ���
	�ڡ�������'������LCDM_mcmc, x;(xΪ0����1����.pro�ļ���ͷ��ע��)��
3)�õ�contourͼ(LCDMSN_mc.ps, LCDMHz_mc.ps...)��	
NOTE: since Mar 2012, the project file(coco.dsp, coco.dsw) will no longer be given. You can still run coco using CVF: adding all coco .f90 files to a blank project and compiling coco.f90, you will get coco.dsp and coco.dsw!

2-Linux
1)����cocoĿ¼��
	�༭coco.f90�ļ���ѡ���Ƿ�ʹ��mcmc������	
	�༭readdata.f90�ļ���������ݻ���ע�͵�����Ҫ������(��ReadInObsData�����н��У����磬��ʹ��sn��ע�͵�'call read_sn')��
	�༭settings.f90�ļ�������ģ�ͺͲ������������Ҫ��Щʱ���һ������ļ����������˼���������Ҫ���õı�����
	����io.f90�ļ��е�plotdir������plotdir='./plot/'(��Ҫ�Ƚ���һ��plot�ļ���)�����ĵĻ�����������coco�ļ��У�
	make��
2)�����ɵ�.pro�ļ�����LCDM_mcmc.pro������Ŀ¼�¿���idl��
	�����ļ����磻
	����LCDM_mcmc, x;(xΪ0����1����.pro�ļ���ͷ��ע��)��
3)�õ�contourͼ(LCDMSN_mc.ps, LCDMHz_mc.ps...)��	
