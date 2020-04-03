z2m (Zoom G3 to midi foot controller)

z2m��Zoom G3�܂���Zoom G3X���A���zmidi�P�[�u������邱�ƂŁA�C�ӂ�DAW��
midi�t�b�g�R���g���[���Ƃ��Ďg�p���邱�Ƃ��\�ɂ���\�t�g�E�F�A�ł��B

# �K�v�Ȃ���
Zoom G3(ver2.10) �܂��� Zoom G3X(ver2.10)
loopMIDI(http://www.tobias-erichsen.de/software/loopmidi.html)

# �g�p���@
1. Zoom G3��ŁA���ׂẴG�t�F�N�g���uT Scream�v�ɐݒ肵���p�b�`��p�ӂ���B
2. Zoom G3��PC��USB�P�[�u���Őڑ�����B
3. loopMIDI���N�����AName���uloopMIDI Port�v�ł��鉼�zMIDI�P�[�u�����L�邱�Ƃ��m�F����B�Ȃ���΍쐬����B
4. Zoom G3�̂��ׂẴG�t�F�N�g�̃X�C�b�`���I�t�ɂȂ��Ă��邱�Ƃ��m�F����B
5. z2m.exe�����s����B
6. �y�_���𓥂ނ�loopMIDI��midi���b�Z�[�W��������B
7. �e�����L����DAW��G�t�F�N�g�\�t�g�E�F�A�̐ݒ������B

# �������
�y�_���𓥂ނƂ��̈ʒu�ɑΉ�����MIDI���b�Z�[�W�����zMIDI�|�[�g�ɑ΂��đ�����B
�����ݒ�ł͍������珇�� B0 00,B0 01,B0 02,B0 03,B0 04,B0 05 ��������B
���̓�B0�̕����Ɋւ��ẮAconfig.ini����STATUS_BYTE�̒l��ύX���邱�Ƃɂ���ĕύX�\�B
�y�_���̃I���I�t�Ɋւ�炸�A�X�C�b�`�𓥂ނƓ����M�������M�����B

���L����f�o�C�X��Zoom G3X�̏ꍇ�́ASTART_SYSEX��
 [0x52,0x00,0x59,0x50]
�ƕύX���Ă��������B
�܂�MIDI OUT�ɔC�ӂ̖��O�̃|�[�g��f�o�C�X���g���ꍇ���A
����ɍ��v����悤�� OUTPUT_DEVICE_NAME �̒l��ύX���Ă��������B

# �R���^�N�g
�ӌ��A�v�]�A�s���������ꍇ�͈ȉ����B
http://blog.livedoor.jp/carling_65/
https://twitter.com/LunarExcursion

# �Q�l�ɂ����T�C�g �g�p�������C�u����
1.
ZOOM G3X(v2.10)��MIDI�R���g���[���[�Ƃ��Ďg�� - ���ڂ�����
https://tpcbtw.hatenablog.com/entry/2018/06/09/173129

2.
GitHub - gesellkammer/rtmidi2: python bindings to rtmidi allowing to listen to multiple ports simultaneously
https://github.com/gesellkammer/rtmidi2

3.
Python��MIDI�t�F�[�_�ƒʐM���郁���iMIDI�f�o�C�X��PC) - Qiita
https://qiita.com/Dr10_TakeHiro/items/e6df6c9b59869a74f899


------------------------------------------------


z2m (Zoom G3 to midi foot controller)

The z2m allows the Zoom G3 or Zoom G3X to be used with any DAW and software FX over a virtual midi cable.
This Software allows you to use it as a MIDI foot controller.

# What you need.
Zoom G3(ver2.10) or Zoom G3X(ver2.10)
loopMIDI(http://www.tobias-erichsen.de/software/loopmidi.html)

# Usage
1. prepare a patch with all effects set to "T Scream" on Zoom G3.
2. Connect the Zoom G3 to your PC with a USB cable.
3. Start loopMIDI and confirm that you have a Virtual MIDI Cable whose Name is "loopMIDI Port". If not, create one.
4. Make sure that all effects on the Zoom G3 are switched off.
5. run z2m.exe.
6. When you step on the pedal, a midi message is sent to loopMIDI.
7. Set up your own DAW and effect software.

# Description
When you step on a pedal, a MIDI message corresponding to the position is sent to the virtual MIDI port.
By default, B0 00, B0 01, B0 02, B0 03, B0 04, B0 05 are sent from the left side in order.
The B0 part can be changed by changing the value of STATUS_BYTE in config.ini.
Regardless of whether the pedal is on or off, the same signal is sent when the switch is pressed.

If the device you own is a Zoom G3X, set START_SYSEX to
 [0x52,0x00,0x59,0x50]
You can also use a port or device of any name for MIDI OUT.
Change the value of OUTPUT_DEVICE_NAME to match the value of it.

# Contact.
If you have any opinions, requests, or defects, please contact us below.
https://twitter.com/LunarExcursion

# Reference
1.
ZOOM G3X(v2.10)��MIDI�R���g���[���[�Ƃ��Ďg�� - ���ڂ�����
https://tpcbtw.hatenablog.com/entry/2018/06/09/173129

2.
GitHub - gesellkammer/rtmidi2: python bindings to rtmidi allowing to listen to multiple ports simultaneously
https://github.com/gesellkammer/rtmidi2

3.
Python��MIDI�t�F�[�_�ƒʐM���郁���iMIDI�f�o�C�X��PC) - Qiita
https://qiita.com/Dr10_TakeHiro/items/e6df6c9b59869a74f899
