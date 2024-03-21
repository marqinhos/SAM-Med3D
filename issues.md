# 1-Error:
```bash
Traceback (most recent call last):
  File "/home/marcos/Marcos_PhD/SAM-Med3D/train.py", line 510, in <module>
    main()
  File "/home/marcos/Marcos_PhD/SAM-Med3D/train.py", line 469, in main
    trainer.train()
  File "/home/marcos/Marcos_PhD/SAM-Med3D/train.py", line 362, in train
    epoch_loss, epoch_iou, epoch_dice, pred_list = self.train_epoch(epoch, num_clicks)
  File "/home/marcos/Marcos_PhD/SAM-Med3D/train.py", line 283, in train_epoch
    for step, (image3D, gt3D) in enumerate(tbar):
  File "/home/marcos/Marcos_PhD/SAM-Med3D/.env/lib/python3.10/site-packages/tqdm/std.py", line 1181, in __iter__
    for obj in iterable:
  File "/home/marcos/Marcos_PhD/SAM-Med3D/.env/lib/python3.10/site-packages/prefetch_generator/__init__.py", line 112, in next
    success, next_item = self.queue.get()
  File "/usr/lib/python3.10/queue.py", line 171, in get
    self.not_empty.wait()
  File "/usr/lib/python3.10/threading.py", line 320, in wait
    waiter.acquire()
  File "/home/marcos/Marcos_PhD/SAM-Med3D/.env/lib/python3.10/site-packages/torch/utils/data/_utils/signal_handling.py", line 66, in handler
    _error_if_any_worker_fails()
RuntimeError: DataLoader worker (pid 417885) is killed by signal: Aborted. 
```