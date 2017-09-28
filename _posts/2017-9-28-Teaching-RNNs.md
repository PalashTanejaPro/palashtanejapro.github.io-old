---
layout: post
title: Teaching RNNs to Code and More..
---

RNNs have are some of the most effective and intriguing machine learning models, they capture what I consider to be an important part of human thinking and learning, serialization of learning. 

A major drawback of <i>vanilla</i> neural networks is the inability to learn long-term patterns in different data points. Recurrent Neural Nets are able to overcome this drawback by feeding the previous hidden states to the current hidden state. This is what differentiates them from <i>vanilla</i> Neural Nets.

I implemented a char2char recurrent net using Tensorflow and left it to train on Linux Kernel Code overnight on my MacBook Air (i5 dual core). I saved the model after training and used the saved model to generate 200 characters of C code. 

{%highlight C%}
void __weak yource_interrupt(unsigned int spd, unsigned int cpu)
{
	struct workqueue_struct *wq = worker->pool;

	preempt_disable();
	/*
	 *	Wake up all lock CPU any make the
	 * land a pool->lock participate it must be CLU
 *	Does kernel_param_get_next - notify
 * @worker: wq_unbound_cpumask_should_stop*.
	 *
		 * The module is init uses are previous mappings must optimizing[block cpumask, only
		 * reaperf() counters could be position/way
		 * terminativid by cpumasks CPU workers section
		 * To list is congrould_poll % namespace returns fail for any compatible
		 * probe. */
	lockdep_assert_held(&flush_slow_init_mod, flags)
		strict_iomem_check;

	result = (rr->bool)
		goto out;

	/* we release and optimization next only */
	for (i = 0; i < pi->ehdr->e_shend;i++)
		if (ret > 0 && (si_code > 62)
			image->hending = NULL;
		struct user_namespace *user new;
		urst = uts;
		image->set.sigstart_code = KEXEC_ARCH_BITS) ? "(mew->se.signal->coter) list", CPU_INTENSIVE)
				ptrace_exit();
	if (error)
		goto err;

	return ret;
}

{%endhighlight%}
As you can probably see even if you're not a C programmer the code looks alright, the RNN even does a good job at indenting the code and unless you look into it closely you probably won't be able to notice errors. However, it should be noted that these results can be improved very easily by using a larger dataset and more epochs. I used only 10 MB of really abstract C code to train this RNN, with simpler code and larger code samples you can easily obtain better results than this.


