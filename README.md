```bash
vmkfstools -i /vmfs/volumes/datastore1/SCOmfg/sco-unix-5.0.7-1.vmdk /vmfs/volumes/datastore1/SCOmfg/SCOmfg.vmdk -d thin
```
คำสั่งนี้จะทำการโคลนไฟล์ .vmdk เดิมไปเป็น SCOmfg.vmdk ในรูปแบบ Thin Provisioned ตามที่คุณต้องการครับ

```bash
vim-cmd solo/registervm /vmfs/volumes/Datastore1/MyNewVM/MyNewVM.vmx
```
คำสั่งนี้จะส่งคืน VMID (Virtual Machine ID) ของเครื่องเสมือนใหม่



นำไฟล์ .vmx วางไว้ใน folder และแก้ไขค่า vmdx ต่างๆให้ตรงกับ vmdx file ที่ใช้
