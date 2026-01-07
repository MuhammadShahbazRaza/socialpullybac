web: gunicorn video_downloader.video_downloader.wsgi:application --bind 0.0.0.0:$PORT --workers 1 --timeout 300 --log-level debug --access-logfile - --error-logfile -
release: python video_downloader/manage.py check && python video_downloader/manage.py migrate --noinput && python video_downloader/manage.py collectstatic --noinput
