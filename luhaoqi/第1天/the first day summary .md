1�˽�RTT���߳���ظ���
2�̵߳Ĵ�����ʹ��
	2.1��̬��������Ҫ��ǰ�����ýṹ������飬����ǰ���������ռ�
	rt_err_t rt_thread_init(struct rt_thread *thread,
                        const char       *name,
                        void (*entry)(void *parameter),
                        void             *parameter,
                        void             *stack_start,
                        rt_uint32_t       stack_size,
                        rt_uint8_t        priority,
                        rt_uint32_t       tick)
    2.2��̬��������Ҫ��������������պ������صľ������ϵͳ���ݿռ��С�Զ�����ռ�
    rt_thread_t rt_thread_create(const char *name,
                             void (*entry)(void *parameter),
                             void       *parameter,
                             rt_uint32_t stack_size,
                             rt_uint8_t  priority,
                             rt_uint32_t tick)
3��Ӳ��ʱ����ʹ��
    Ӳ����ʱ���� ��Ҫ����Ӳ����ʱ����systick��timx���ȣ���Ҫ�ڶ�ʱ���ж��й���
    �����ʱ���� ��ʱ����ֻ��Ҫ���߳��й����ɡ�
4RTT����������
    4,1Resrt_Handler����startup_enter��
    4.2�Ƚ���SystemInit����������SystemClockCinflg����ִ��ϵͳʱ��
    4.3�ٽ���entry����,����rttthread_startup����ִ�г�ʼ���������ر��жϣ����������ʼ������ӡ��Ϣ����ʱ����ʼ�����û������ʼ�����������񣬿�ʼ���ȣ�
