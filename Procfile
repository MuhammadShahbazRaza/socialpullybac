web: cd video_downloader && gunicorn video_downloader.wsgi:application --bind 0.0.0.0:$PORT --workers 1 --timeout 300 --log-level debug --access-logfile - --error-logfile - --capture-output --enable-stdio-inheritance
release: cd video_downloader && python manage.py check && python manage.py migrate --noinput && python manage.py collectstatic --noinput
