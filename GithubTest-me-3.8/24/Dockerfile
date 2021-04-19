FROM python:3.8
ADD VideoPose3D VideoPose3D
RUN ["pip","install","torch"]
RUN ["pip","install","androidviewclient"]
RUN ["pip","install","numpy"]
RUN ["pip","install","matplotlib"]
RUN ["pip","install","common-utils"]
CMD cd VideoPose3D && python run.py -k cpn_ft_h36m_dbb -arc 3,3,3,3,3 -c checkpoint --evaluate pretrained_h36m_cpn.bin

