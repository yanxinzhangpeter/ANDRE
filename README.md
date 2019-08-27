# ANDRE

The empty-label-malware file records Android malware hash values with an empty label processed by AVClass and Euphony.

The controversial-label-malware file records the hash values that the labels of Android malware are controversial after being processed by AVClass and Euphony.


How to use:

1. The user can search for the corresponding raw labels of the malware hash value in the Virustotal according to the hash value in the empty-label-malware and controversial-label-malware. These raw labels will be entered as features in our model.

2. According to the hash value list, all malware is downloaded. After downloading, use dex2jar to convert all dex files in apk files to jar file format.

3. After getting all the jar files, use SourcererCC to calculate the similarity between all malwares. 

4. Select all malware pairs with a similarity greater than 85% and record them as the second feature of our method.
