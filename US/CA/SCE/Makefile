FILES=$(shell find . -name '*.dlp' -print)
TARGETS=$(addsuffix .glm,$(basename $(FILES)))

all: $(TARGETS)

clean:
	rm *.{glm,csv}

%.glm: %.dlp
	gridlabd python -m read_dlp $<