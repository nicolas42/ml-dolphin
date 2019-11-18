
Install

	git clone https://github.com/AlexeyAB/darknet
	cd darknet
	make

get some premade training weights

	wget https://pjreddie.com/media/files/darknet53.conv.74


*** Copy all the files in this directory into the darknet directory ***

Train

	./darknet detector train obj.data obj.cfg darknet53.conv.74 -map

Test

	./darknet detector test obj.data obj.cfg obj.weights dataset/img_456.jpg



copy from ec2
scp -r -i ~/.ssh/id_rsa.pub ubuntu@13.236.66.105:/home/ubuntu/output ~/output

test weights

./darknet detector test cfg/obj.data cfg/obj.cfg obj_11000.weights darknet_training_demo/nfpa_dataset/pos-1.jpg


test weights
./darknet detector test obj.data obj.cfg obj_11000.weights pos-286.jpg





