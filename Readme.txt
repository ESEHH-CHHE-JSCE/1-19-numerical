���1.19�T���v���R�[�h�ɂ���

���Y�t�ꗗ
�@���̃T���v���ɂ͈ȉ��̃t�@�C�����܂܂�܂��D

�E�ucommon.h�v�ꕔ�̕ϐ����w�肵���w�b�_�t�@�C��
�E�ucondition.d�v�v�Z�����ݒ�t�@�C��
�E�uboundary.d�v���E�����ݒ�t���O�L�q�t�@�C��
�E�ugrid.f�v�v�Z�i�q�쐬�v���O�����\�[�X�R�[�h
�E�udensity2d.f�v����2�������x����̓v���O�����\�[�X�R�[�h
�E�ucsvdata.f�v

�����ӎ���
�udensity2d.f�v���̈ڗ����v�Z�T�u���[�`���ucip_cal�v�͉��L�̎Q�l�����Ɋ�Â��܂��D
��F�C���C���s�C���`�z��F�uCIP�@�v�C�X�k�o�Ŋ�����ЁC2003.

���g�p�̎菇

�P�j��L�́ugrid.f�v���R���p�C�����Ď��s���邱�ƂŁC�ucommon.h�v�C�ucondition.d�v�C����сuboundary.d�v�ɋL�q���ꂽ�����ɉ����Čv�Z�i�q���쐬�����D
�v�Z�����ɗp�����ϐ��ɂ��Ă͉��L�̂Ƃ���ł���D

���ucommon.h�v�ݒ�ϐ��ɂ���
im,jm�Fx�����Cz�����ɗp�ӂ���z�񐔁C�v�Z�i�q�̐��ɋ��E�����p�̔z����v���X������

���ucondition.d�v�ݒ�ϐ��ɂ���
nx,nz�Fx���������z�����i�q��
iscf�F�\�[�X�ӏ��ݒ�̗L��
chleng,height�F���H������ї��H����
g,rho,rnu,diffyr�F�d�͉����x�C���ӗ��̖̂��x�C���S���W���C�g�U�W��/���S���W���̔�
tuk,etime,dt�F�v�Z���ʏo�͎��ԍ��݁C�v�Z�I�������C�v�Z���ԍ���
lsor,soralp�F���͂̌v�Z�̔������C���͌v�Z�̊ɘa�W��
pretime�F������������̊ɘa�ɂ����鎞��

���uboundary.d�v�ݒ�ϐ��ɂ��āi�����Ƃ��ĕύX�s�v�j
ib1u,ib1w,ib2u,ib2w�F�㗬����щ������E�̗��������̋��E�����ݒ�p�t���O
ib3u,ib3w,ib4u,ib4w�F��ʂ���щ��ʋ��E�̗��������̋��E�����ݒ�p�t���O
ib1p,ib2p,ib3p,ib4p�F���͌v�Z�̋��E�����ݒ�p�t���O
ib1r,ib2r,ib3r,ib4r�F�Z�x�v�Z�̋��E�����ݒ�p�t���O

���ugrid.f�v�ݒ�ϐ��ɂ���
�E84�s�ڂ���88�s��
c     boundary settings
      do k=1,nz
          bc1_u(k)=1.5
          bc2_u(k)=1.5
      end do

�@bc1_u(k)�Cbc2_u(k)�ɂ�苫�E�㉺���̗�����ݒ�

�E90�s�ڂ���95�s��
c     initial settings
      do i=0,nx
        do k=1,nz-1
            u_l(i,k)=1.5
        end do
      end do 

�@�̈���̗���̏����l��ݒ�

�E97�s�ڂ���109�s��
c     source settings
      do i=50,50
        do k=50,52
            isw_w(i,k)=1
            scw_w(i,k)=-5.0
        end do
      end do
      do i=50,50
        do k=50,52
            isr_c(i,k)=1
            scr_c(i,k)=rho-1.5
        end do
      end do

�@���x�����\�[�X�̈ʒu�Ɨ���������

�Q�j���̌�C�udensity2d.f�v���R���p�C�����Ď��s���邱�ƂŁC�v�Z���ʂ𓾂�D

�R�j���̎��ɐ������ꂽ�t�@�C���Q�ɑ΂��C�ucsvdata.f�v���R���p�C�����Ď��s���邱�ƂŁC�o�͎��ԍ��݂Ő������ꂽ�Z�x����ї����x�N�g��������csv�`���̌��ʃt�@�C���Q���쐬�����D


���������

�����R�[�h��Windows10Pro���Intel oneAPI 2021�ɂ�铮����m�F���Ă���D
