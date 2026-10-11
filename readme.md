# [SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm with MATLAB Code

MATLABSimulation resultsclear all;  close all; clc;\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n%   CSA Imaging Algorithm\n%    For Stanley Park & city,        use range = 1850, azimuth =7657\n%   first_rg_cell    =  1850;      % Define the range limits\n%  first_rg_line     =  7657;      % Define the azimuth limits (19432 max)\n%  Nrg_cells       =  2048      % Suggest 2048 cells\n%  Nrg_lines_blk  =  1536;       % Suggest 1536, it should be larger than the\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n​\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n%    Preliminary: Read data, the data is provided by the website and extracted the imaging area needed.\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\nload CDdata1.mat\ndata=double(data);          % Convert data to double type\n[length_a,length_r]=size(data);    % Get the size of the data\n​\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n% Step 1: Azimuth-directional Fourier transform, transforming the baseband signal to the range Doppler domain\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n% Step 2: Multiply the Doppler domain signal with the linear variable-scale equation.\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n​\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n% Step 3: Distance-Doppler Transform to 2D Frequency Domain from Distance Doppler Domain\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n% Step 4: Complete (distance compression, SRC, consistent RCMC) through a phase multiplication.\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n% Step 5:   Distance-to-Frequency Inverse Fourier Transform, returns to the distance Doppler domain.\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n% STEP6: Complete phase correction + azimuth matching filtering\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n​\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n%   STEP7:   Complete the azimuth-directional Fourier inverse transformation\n%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%\n​\n  

## Images

![[SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm [with MATLAB Code]](01.jpg)
![[SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm [with MATLAB Code]](02.jpg)
![[SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm [with MATLAB Code]](03.jpg)
![[SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm [with MATLAB Code]](04.jpg)
![[SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm [with MATLAB Code]](05.jpg)
![[SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm [with MATLAB Code]](06.jpg)
![[SAR Imaging] Vancouver SAR Imaging Based on CS Algorithm [with MATLAB Code]](07.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
