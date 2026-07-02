Here are my notes on what I did to fix the Raman.

# Camera: 
Ed donated a camera: [Celestron – 5MP CMOS Digital USB Microscope Imager – Digital Camera Captures Hi-Res Images and 30FPS Video – Perfect for Science Education and Classroom](https://www.amazon.com/dp/B01G7J0688?ref=cm_sw_r_cso_cp_apin_dp_E7N82NNBHB91HS71XQSV&ref_=cm_sw_r_cso_cp_apin_dp_E7N82NNBHB91HS71XQSV&social_share=cm_sw_r_cso_cp_apin_dp_E7N82NNBHB91HS71XQSV&rsd=0%2BcftzIgRaJQ5qiyL986z%2BidSb30al9Nbl5QZLL9wHbHaT0BHN62rCKmGdR0HNNLMjgyd15qdyqoZUNXFk39UXnEzzgryoA5dBMiTHVORyQamXfeZA%3D%3D&edk=AQIDAHi1lw%2FM8UbbSMD9ScOOFEmBMHMthHeEhqDaQYPJUAX3jQE2yj2t%2BBTV0GgIooCm9gRsAAAAfjB8BgkqhkiG9w0BBwagbzBtAgEAMGgGCSqGSIb3DQEHATAeBglghkgBZQMEAS4wEQQMyhSac9z2BF39PRxZAgEQgDsDLizEZ14xmm0QAYXqrzbpe88HR31fRNVt2B6pd5D%2BuptepICrp4lqB2qIbRri8UyC3wqBRqd9ZIS0LA%3D%3D)
# CCD: 
The CCD was broken (image sensor was deemed broken) and I shipped it as RMA 19212 to ATIK (the invoice is attached)[Invoice 382.pdf](https://github.com/user-attachments/files/29605063/Invoice.382.pdf)
We can use the Artemis software to get a picture of the whole CCD.

# Galvo scanner
I had problems with the galvo scanner that the +15V signal was intermittant (sometimes working sometimes not)
<img width="314" height="499" alt="image" src="https://github.com/user-attachments/assets/4ecb3136-b7e8-438c-9192-b20ec7e6ef88" />
Surprisingly, I found another galvo scanner in the lab after cleanup and that one works perfectly.

# Software
The galvo can be controlled in the NanoSpectrum version 1.8 but I haven't found the control in 1.7.2.3
The CCD is an Artemis and using a patch I got it to work in 1.7.2.3 (haven't tried newer versions).
The camera is not original and doesn't seem to work with 1.8 but we can just use the windows camera app to operate it.

# Beam path
the system has a scan lens that may be misaligned but centering is hard because the beam is moving with the galvo rotation.
<img width="740" height="442" alt="image" src="https://github.com/user-attachments/assets/986e2ac1-f859-4385-8745-1f5740c2c6dd" />

# Results
I made Rhodamine 6G solution (1mg/ml) and put it in the beam path (under the objective and in front of the scan lens) and get strong luminescence after optimizing the mirror in front of the spectrometer slit.

<img width="1915" height="1030" alt="image" src="https://github.com/user-attachments/assets/91759d19-f454-4738-bc2a-d6e91e91cf67" />

Also, using Naphtalene in front of the scan lens gets signal.
<img width="1920" height="1440" alt="image" src="https://github.com/user-attachments/assets/3f84aa59-8d13-46ea-97b5-12a8afc42c96" />
