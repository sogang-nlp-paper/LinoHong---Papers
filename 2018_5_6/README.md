
5.05 - 05.10 : # Seq2Seq # Copying Mechanism # Generation
============
	
1. '심층학습을 이용한 기계번역 연구동향', 이건일, 이종혁. 정보과학회, 2015
	read 05.10 - 05.15


5.18 - 05.23 : # Seq2Seq # CNN or RNN Encoder Decoder. # Kalchbrenner # ByteNet
============

1. 'Neural Machine Translation in Linear Time', Kalchbrenner et al. arXiv, 2017.
2. 'Recurrent continuous translation models.', Kalchbrenner & Blunsom. EMNLP, 2013.
	read both 05.18 - 05.23 

06.01 - 06.05 : # Question Generation # Reading Comprehension # Summarization
============

1. 'Learning to Ask: Neural Question Generation for Reading Comprehension', Xinya Du et al. ACL, 2017.
	- use Seq2Seq (Attention mechanism) to encode sentence and paragraph. Use both of the encoded information
	  to decode, generating a question.
	- data set of SQuAD. 
2. 'Get To The Point: Summarization with Pointer-Generator Networks', Abigail See et al. ACL, 2017.
	- use seq2seq + attention to encode document into a representation.
	- use pointer-generator network to decide probability of generation and copying. This mechanism solves
	  UNK problem.
	- use Coverage mechanism to cover already generated sentences. 
	- analyses why extractive method scores higher ROUGE point than abstractive 
		=> simple word matches from reference summarization.
	- analyses what pointer-generator contributes to the summarization result
		=> It increases ROUGE point, but less abstractive. 
		=> future work
