Training:
> python train.py --input_dir='./data/' --output_dir='./output/' --model_save_dir='./model/' --batch_size=64 --epochs=3000 --number_of_images=1000 --train_test_ratio=0.8
    
Testing:
1. Test Model- Here you can test the model by providing HR images. It will process to get resulting LR images and then will generate SR images. And then will save output file comprising of all LR, SR and HR images.        
> python test.py --input_high_res='./data_hr/' --output_dir='./output/' --model_dir='./model/gen_model3000.h5' --number_of_images=25 --test_type='test_model'
       
           
2. Test LR images- This option directly take LR images and give resulting HR images.
> python test.py --input_low_res='./data_lr/' --output_dir='./output/' --model_dir='./model/gen_model3000.h5' --number_of_images=25 --test_type='test_lr_images'
      
