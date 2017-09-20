# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Dockerfile                                         :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: sjones <sjones@student.42.us.org>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2017/09/20 16:02:36 by sjones            #+#    #+#              #
#    Updated: 2017/09/20 16:24:24 by sjones           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

FROM debian:latest

RUN apt-get update &&\
	apt-get -y install\
		build-essential\
		git\
		python-dev\
		python-pip\
		libopencv-dev\
		python-opencv

RUN pip install tensorflow

RUN git clone https://github.com/mpatacchiola/deepgaze.git &&\
	cd deepgaze\
	python setup.py install

CMD /bin/bash


